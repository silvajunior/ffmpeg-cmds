# FFMPEG cmds
![](https://raw.githubusercontent.com/silvajunior/ffmpeg-cmds/refs/heads/main/ffmpeg.webp)
Commands FFMPEG

Cortar:
```bash
ffmpeg -i input_video.mp4 -ss 00:00:00 -to 00:00:10 -c copy output_video.mp4
```
Converter:
```bash
ffmpeg -i entrada.mp4 saída.avi
```
Forçar a taxa de quadros:
```bash
ffmpeg -i entrada.avi -r 24 saída.mp4
```
Definir a taxa de bits do vídeo:
```bash
ffmpeg -i entrada.avi -b:v 64k -bufsize 64k saída.mp4
```
Extrair o Áudio Original de um Vídeo.
```bash
ffmpeg -i output_video.mp4 -vn -acodec copy audio_original.aac
```
Extrair o Vídeo Original (Sem Áudio)
```bash
ffmpeg -i output_video.mp4 -an -vcodec copy video_original.mp4
```
Juntar o Vídeo Original e o Áudio Original (Recombinar):
```bash
ffmpeg -i video_original.mp4 -i audio_original.aac -c:v copy -c:a copy output_video_combined.mp4
```
