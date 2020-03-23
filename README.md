# Инструкция по добавлению карты распространения коронавируса
<p align="center">
<img src="https://avatars.mds.yandex.net/get-bunker/56833/13634d10eba08e395b1133c6743c24517b433ecb/orig" width="650px" />
</p>

Чтобы добавить карту распространения коронавируса к себе на сайт, необходимо в html код страницы добавить тег:

```html
<iframe src="https://yandex.ru/maps/covid19?embed=covid" width="800px" height="500px"></iframe>
```

Если хочется добавить только карту без панели со сводными данными по России, параметр `embed=covid` нужно заменить на `embed=covid-map`:

```html
<iframe src="https://yandex.ru/maps/covid19?embed=covid-map" width="800px" height="500px"></iframe>
```
<img src="https://avatars.mds.yandex.net/get-bunker/49769/e60f352964bc59a4a0b95005104b16fbdf5eb23a/orig" width="300px" />
