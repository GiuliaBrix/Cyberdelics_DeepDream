Cyberdelics DeepDream

A short video exploring DeepDream-style visuals.

File: Cyberdelics_DeepDream.mp4
Duration: about 10 min 40 s
Resolution: 480p
Size: about 18 MB

Tip: GitHub plays .mp4 files directly in the browser when you click on them.

About
<!-- Add the story behind the video: what it shows, how it was made, what inspired it. -->
Author: Giulia Brizzi
Year: 2026
Tools used: DeepDream (add the exact tool or model here)
Compression notes

The original file was about 60 MB. It was compressed with ffmpeg using two-pass H.264 encoding to fit under 20 MB:

bash
ffmpeg -y -i Cyberdelics_DeepDream.mp4 -c:v libx264 -b:v 170k -vf scale=-2:480 -pass 1 -an -f null /dev/null
ffmpeg -y -i Cyberdelics_DeepDream.mp4 -c:v libx264 -b:v 170k -vf scale=-2:480 -pass 2 -c:a aac -b:a 64k output.mp4

Because DeepDream footage is full of fine detail, the compressed version loses some sharpness compared to the original.

License
<!-- Choose a license, for example CC BY 4.0: https://creativecommons.org/licenses/by/4.0/ -->

All rights reserved unless stated otherwise.
