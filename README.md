# youtube-playlist-download
Как скачать одной командой целый плейлист с ютуба? С помощью python, ffmpeg и yt-dlp.

![image](https://github.com/rumiantsevaa/youtube-playlist-download/assets/89034072/104d896b-b373-4d0d-ae1e-2500bf552c80)

# Скачивание видео с YouTube

Эта инструкция позволяет скачивать видео с YouTube в формате MP4

## Требования

Для использования этого скрипта вам понадобится:

1. Python 3.6 или выше
2. yt-dlp
3. ffmpeg

## Установка

1. Установите Python с официального сайта: https://www.python.org/downloads/
   При установке обязательно отметьте галочку "Add Python to PATH".

![image](https://github.com/rumiantsevaa/youtube-playlist-download/assets/89034072/3a482f4e-9259-4df1-b3d8-c10e7f6aa261)


2. Установите yt-dlp через pip:
pip install yt-dlp

![image](https://github.com/rumiantsevaa/youtube-playlist-download/assets/89034072/06bf53bd-6e98-4336-b6e7-a7e3fd572989)


4. Скачайте и установите ffmpeg с официального сайта: https://ffmpeg.org/download.html

![image](https://github.com/rumiantsevaa/youtube-playlist-download/assets/89034072/b0aa287e-7185-4bc1-8af3-5d9b512ef175)


Добавьте путь к ffmpeg в переменную PATH вашей системы.

## Использование

1. Откройте терминал или командную строку.

2. Перейдите в папку в терминале, куда вы хотите сохранить видео.

3. Выполните следующую команду:
yt-dlp -f "bestvideo[height<=360][ext=mp4]+bestaudio[ext=m4a]/best[height<=360][ext=mp4]/best[height<=360]" --merge-output-format mp4 [URL_ПЛЕЙЛИСТА]

Замените [URL_ПЛЕЙЛИСТА] на URL вашего YouTube плейлиста.

## Примечание

- Видео будут скачаны в папку, из которой был открыт терминал.
- Формат видео: MP4
- Если видео с указанными параметрами недоступно, будет выбрано наилучшее доступное качество, не превышающее 360p.
