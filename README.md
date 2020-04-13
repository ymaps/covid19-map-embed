# Инструкция по добавлению карты распространения коронавируса или карты самоизоляции

## Карта распространения коронавируса
<p align="center">
<img src="https://avatars.mds.yandex.net/get-bunker/56833/13634d10eba08e395b1133c6743c24517b433ecb/orig" width="650px" />
</p>

### Десктоп версия
Чтобы добавить карту распространения коронавируса к себе на сайт, необходимо в html код страницы добавить тег:

```html
<iframe src="https://yandex.ru/maps/covid19?embed=covid" width="800px" height="500px"></iframe>
```

Если хочется добавить только карту без панели со сводными данными по России, параметр `embed=covid` нужно заменить на `embed=covid-map`:

```html
<iframe src="https://yandex.ru/maps/covid19?embed=covid-map" width="800px" height="500px"></iframe>
```
<img src="https://avatars.mds.yandex.net/get-bunker/49769/e60f352964bc59a4a0b95005104b16fbdf5eb23a/orig" width="300px" />

### Мобильная версия

Для добавления карты на мобильную версию сайта, в теге iframe необходимо использовать ссылку с параметром `embed=covid-map`:
```html
<iframe src="https://yandex.ru/maps/covid19?embed=covid-map" width="500px" height="450px"></iframe>
```
## Карта самоизоляции

Чтобы вставить на сайт карту самоизоляции, вместо карты расптространения коронавируса, нужно использовать те же айфреймы, что и выше, только заменить ссылку в аттрибуте `src`:
1. Для карты без панели: `https://yandex.ru/maps/covid19/isolation?embed=covid-map`
2. Для карты с панелью: `https://yandex.ru/maps/covid19/isolation?embed=covid`

Также во всех ссылках можно использовать стандартные параметры яндекс карт для выбора нужной области карты: `ll` — для координаты центра карты, `z` — для уровня зума. 

Самый простой способ вставить нужную область в iframe: 
1. Открыть карты по ссылке https://yandex.ru/maps/covid19/isolation?embed=covid-map 
2. Отцентрировать карту и выбрать нужный зум
3. Скопировать ссылку из адресной строки в iframe
