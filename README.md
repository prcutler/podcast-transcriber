# podcast-transcriber
Audio transcription based on [Assembly AI's Python in 5 Minutes tutorial](https://github.com/AssemblyAI-Examples/assemblyai-and-python-in-5-minutes)

This adds SRT export in addition to the TXT transcription.  After running `transcribe.py` two files will be saved:
* transcript.txt
* subtitles.srt

## TO-DO
- [ ] Automatic filename based on MP3 filename

## Requirements

```console
$ pip install requests
```

## Usage:

If your AssemblyAI API key is stored as an environment variable called `AAI_API_KEY` file, then you can omit the optional `--api_key` argument.

```console
$ python transcribe.py audio_file [--local] [--api_key=<YOUR-API-KEY>"]
```

Example for hosted file:

```console
$ python transcribe.py https://github.com/AssemblyAI-Examples/assemblyai-and-python-in-5-minutes/raw/main/audio.mp3 --api_key=<YOUR-API-KEY>
```

Example for local file:

```console
$ python transcribe.py audio.mp3 --local --api_key=<YOUR-API-KEY>