# add_subtitles

I'm really particular about subtitles. When I'm watching movies I want them there, but if they're a little out of sync it's annoying.

However, ffmpeg does not allow you to shift subtitles while adding them to a video track. So, I made this script which automates the process of
constructing a new subtitle track with shifted timings, attaching that to a video file, and then cleaning up the temporary file.

You can specify the timing shift and language code for an attached subtitle track. If you have subtitles that are already aligned just don't
specify a delay and the script will attach the subtitles as-is. The language code is also optional but defaults to 'eng' (for English), so if
your subtitles are in a different language then you'll need to provide the proper language code.
