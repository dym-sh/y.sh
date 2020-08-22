# y

> algorithmically-enhanced [youtube-dl](https://yt-dl.org) wrapper for audio-downloads


## use
`y <URL>`

> `y https://orax.bandcamp.com/track/ectoplasmic`

(edit to set your prefered save-files paths)


## requires
- `pip install youtube_dl` – the main thing, you should already have it
- `sudo apt install -y ffmpeg` – to convert files of diffrent formats
- `cargo install sd` – better `sed`
- `sudo apt install -y lynx` – to easily scrap web-pages


## site-specific improvements

### bandcamp
1. prefers mp3-320 (checks every track)
2. downloads entire discography if given root-domain or `/music` url

### twitter
file-names are just twitter-username and tweet-number
(instead of full text of a tweet, which can result in strings over 255 characters long, aborting the entire process)

### youtube
allows to set several predetermined filesystem-paths to keep file-categories separately:

- `y m <youtube_URL>` – music (automatically chosen for `music.youtube.com`)
- `y c <youtube_URL>` – comedy-tracks
- `y a <youtube_URL>` – audiobooks

### soundcloud
1. occasional wav-files are converted to mp3 320kb/s
2. artist is set based on url (instead of having none by default)


## mirrors
- [github](https://gituhb.com/dym-sh/y-sh/)
- [src.dym.sh](https://src.dym.sh/y-sh/)
- [hyper](hyper://4329bfffa5700e21bb0c89db374590c4b39d57b21a19aa1dc8677882e59c3cf4/lab/y-sh/) [[?](https://beakerbrowser.com)]

## license
[MIT](./LICENSE)
