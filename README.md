This is the source code for two projects I made with Epstein files. The files are heavily
redacted and the diverse blobs of redactions can be used to make a lot of things. I hope
this repo raises awareness of the opression and tranny of the ruling class via internet
culture.

Uses KNN to match feature vectors of the each image (extracted from pages of pdf) and maps
them accordingly to video input to mimic the outlines of the input video.

Example Usage :

[Doom but the video output is Epstein files](https://www.youtube.com/watch?v=bslvIiDfwag)
[Bad Apple on Real Epstein files](https://www.youtube.com/watch?v=p5iqCKzUhlg)

## To run:

> [!WARNING] 
> Tested on linux w/ x11 only.

1. Install the dependencies from requirements.txt
```bash
pip install -r requirements.txt
```
2. Setup the folder structure in following fashion:

```
❯ tree --gitignore
.
├── doom.py
├── input_pdfs
│   ├── EFTA00005705.pdf
│   ├── EFTA00005707.pdf
│   ├── EFTA00005711.pdf
│   └── EFTA0000XXXX.pdf
├── main.py
└── requirements.txt
```

### Bad Apple:
3. Download Bad Apple and save it as ``bad_apple.mp4`` (use yt-dlp or something)
4. run main.py : ``python main.py``
5. finally use ffmpeg to stich the audio to it:
```bash
ffmpeg -i redacted_apple.mp4 -i bad_apple.mp4 -map 0:v -map 1:a -c:v copy -shortest final_with_audio.mp4
```

It took me ~45min to render on my Ryzen 5 5500U, quite an CPU intensive work. I am sure it
can be optimized but I haven't looked into it.

### Doom
> [!WARNING] 
> Doesn't work with wayland.

3. Download Doom and DOSBOX
4. Change config to make sure input capture is correct
5. run doom.py : ``python doom.py``

Licensed under MIT. 
Check out my website : [theindiandev.in](https://theindiandev.in)
My Discord server : [discord.gg/qEYbuWu5NE](https://discord.gg/qEYbuWu5NE)
