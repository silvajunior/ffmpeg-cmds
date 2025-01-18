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
