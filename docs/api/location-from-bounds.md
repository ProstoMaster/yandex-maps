# getLocationFromBounds

## Параметры

### bounds

Обязательный параметр. Границы, из которых надо получить центр и зум

### map

Обязательный параметр. Инстанс карты, полученный из v-model

### roundZoom

Нужно ли округлять координаты. Полезно, если вам требуется целочисленное значение или просто нужно уменьшить масштаб.

Принимает: `boolean` или `floor`/`round`/`ceil`. Если `true`, то выполнит `Math.floor`.

Также используется как стратегия округления в `comfortZoomLevel`.

### comfortZoomLevel

"Докручивает" уровень зума до комфортного отображения всего, что входит в границы.

Если `true`, то при разнице менее 0.5 вычитает единицу из зума (так, 16.4 станет 15.4, а 16.6 останется без изменений).

В случае, если ранее использовался `roundZoom`, разница будет смотреться из первоначального зума, и пример выше станет таким: 16.4 -> 15, 16.6 -> 16 (при стратегии `floor`).

Также принимает объект с параметрами `diff` (по умолчанию 0.5), `correction` (по умолчанию 1) и `roundStrategy` (по умолчанию: roundZoom или `floor`) для самостоятельной настройки всех параметров.

## Возвращает

Promise, содержащий посчитанные `center` и `zoom`.

> [!IMPORTANT] Важно
> `center` незначительно отличается от того, что возвращает сам Яндекс под капотом. Возможно, они делают что-то ещё, либо это ошибка нашей библиотеки.
>
> `zoom` при этом идентичен на 100%.

## Пример использования

```typescript
import { getLocationFromBounds } from 'vue-yandex-maps';

if (map.value) {
  const {
    center,
    zoom
  } = await getLocationFromBounds({
    bounds,
    map: map.value,
    roundZoom: true, //Выполнить округление зума через Math.floor
    comfortZoomLevel: true, //Добавить "пространства" в зум
  });
}
```