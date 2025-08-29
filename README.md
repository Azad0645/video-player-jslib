# Video Web Player

Видеоплеер с собственным управлением и стилизацией. Основан на библиотеке `Playable`.

![Screenshot.png](screenshots/Screenshot.png)

## Как подключить

Скачайте `player.js` и подключите его вместе с зависимостями:

```html
<script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
<script src="https://unpkg.com/playable@2.10.3/dist/statics/playable.bundle.min.js"></script>
<script src="player.js"></script>
```

Добавьте контейнер с `id="player"` и вложенным элементом `.js-video-container`. Пример:

```html
<div id="player">
  <div class="js-video-container"></div>
</div>
```

Инициализируйте плеер:

```html
<script>
  createPlayer({ elementId: 'player' });
</script>
```

Чтобы указать своё видео:

```html
<script>
  createPlayer({
    elementId: 'player',
    src: 'https://example.com/video.mp4'
  });
</script>
```

## Кнопки управления

`js-video-container` — тег, внутри которого будет размещено само видео.

`js-play-button` — кнопка запуска видео-плеера.

`js-pause-button` — кнопка паузы видео-плеера.

`js-mute-button` — кнопка, которая выключает звук плеера.

`js-volume-button` — кнопка которая включает звук.

`js-fullscreen-button` — кнопка включает полноэкранный режим.

`js-current-time` — внутри тега отобразится текущее время видеозаписи.

`js-duration` — внутри тега отобразится общая продолжительность видеозаписи.

`.js-progress` и `js-progress-slider` — комбинация из двух тегов для отображения ползунка видео-плеера.

Подключите Font Awesome для иконок:
```html
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
```

## Онлайн-демо
Онлайн-демо: