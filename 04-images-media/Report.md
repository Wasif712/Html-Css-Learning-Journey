Q1: <picture>
Responsive/alternative image sources ke liye:
<picture>
<source media="(max-width: 600px)" srcset="images/food-small.jpg">
<img src="images/food-large.jpg" alt="Restaurant special dish">
</picture>
Concept:Ye responsive images ke advanced concepts mein important hai.
Desktop → large image
Mobile → small image

Q2:  Image Formats
Common formats: JPEG / JPG, PNG, SVG, WebP, AVIF, GIF
JPEG — Usually photographs ke liye useful.
PNG — Transparency aur lossless graphics ke liye useful.
SVG — Logos/icons/vector graphics ke liye excellent.
WebP — Modern web image format, generally good compression.
AVIF — Modern image format with strong compression and image quality.

Q3: <figure>
Agar image ek self-contained piece of content hai, especially with caption:
<figure>
<img src="images/biryani.jpg" alt="Chicken biryani served in a traditional dish">
</figure>

Q4: <figcaption>
Image ka caption:
<figure>
<img src="images/biryani.jpg" alt="Chicken biryani served in a traditional dish">
<figcaption>Our famous traditional chicken biryani.</figcaption>
</figure>

Q5: <audio>
HTML audio:
<audio controls>
<source src="audio/restaurant.mp3" type="audio/mpeg">
</audio>
controls browser ko playback controls provide karne ke liye kehta hai.
User ko generally: ▶ Play ,  Volume , Progress jaisi controls mil sakti hain.

:- Audio Formats: Common: MP3, WAV, OGG
Browser support format ke according vary kar sakta hai, isliye <source> useful hai.

Q6: <video>
Basic: <video controls width="800" poster="images/restaurant-poster.jpg">
<source src="videos/restaurant-tour.mp4" type="video/mp4">
</video>
1. Video Attributes
Important attributes: controls , autoplay , muted , loop , poster , width , height ,preload 

Q7: Accessibility — Video
Professional website mein captions important ho sakte hain.HTML <track> use kar sakte hain:
<video controls>
<source src="videos/restaurant-tour.mp4" type="video/mp4">
<track kind="captions" src="captions-en.vtt" srclang="en" label="English">
</video> Ye accessibility ka important concept hai.

Q8: <iframe>
iframe kisi external resource/page ko current page ke andar embed karne ke liye use hota hai. Example:
<iframe src="https://example.com" title="Example website" width="800" height="500"></iframe>
Lekin arbitrary websites iframe embedding block kar sakti hain.


(^ - ^)
IMAGE
│
└── <img>
IMAGE + CAPTION
│
└── <figure>
├── <img>
└── <figcaption>
AUDIO
│
└── <audio>
└── <source>
VIDEO
│
└── <video>
├── <source>
└── <track>
EXTERNAL EMBED
│
└── <iframe>

















