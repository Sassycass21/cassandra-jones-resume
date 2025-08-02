## <audio> Element
Used to embed sound files (like .mp3, .ogg, .wav).

<audio controls>
    <source src="sound.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
    </audio>

🔸 controls displays built-in playback buttons
🔸 Provide a message that appears only if the browser does not recognize the <audio> element. It ensures that users still receive some content or instruction.

## <video> Element
Used to embed videos (like .mp4, .webm, .ogg).

<video width="320" height="240" controls>
    <source src="movie.mp4" type="video/mp4">
    <source src="movie.ogg" type="video/ogg">
    Your browser does not support the video tag
</video>

🔸 controls enables the default video player interface
🔸 width and height set the video display size
🔸 Not all browsers support the same video formats. Using multiple <source> elements increases compatibility.
🔸 The fallback text ensures accessibility if the browser doesn’t support the tag

## Optional Attributes:

autoplay — starts playing automatically (may be blocked)
<audio controls autoplay>

loop — replays the video/audio automatically
<audio controls autoplay loop>

muted — starts playback with sound off
<audio controls autoplay muted>

poster — an image shown before the video plays

Best Practices:

✅ Always include controls so users can interact with the media

✅ Use multiple formats for broader compatibility

✅ Offer captions or transcripts when possible (for accessibility)

❌ Avoid autoplay unless it's muted or crucial to the experience