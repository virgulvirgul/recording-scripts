# Recording-scripts

## How To Use

To clone and run this application, you'll need [Git](https://git-scm.com), [Python3.5](https://www.python.org/downloads/release/python-350/), [FFmpeg](https://www.ffmpeg.org/) and [Streamlink](https://github.com/streamlink/streamlink) installed on your computer. From your command line:

```bash
# Clone this repository
$ git clone git@github.com:Brinnyman/recording-scripts

# Go into the repository
$ cd recording-scripts

# Run the app
$ python3.5 recorder.py [options]
```

```bash
Usage: recorder.py [options]

Options:
-h, --help prints this message
-n, --name <recording directory and twitch username>
-t, --type <twitch, youtube, vod, repair>
-u, --url <youtube-live url>
-v, --vod <twitch vod id code>
```

## Configuration

```
self.root_path = os.path.abspath('')  # recording path
self.ffmpeg_path = ''  # path to ffmpeg executable
self.streamlink_path = ''  # path to streamlink executable
```

## Examples

```bash
Examples:
Recording twitch stream:
recorder.py -name lirik
Recording twitch vod:
recorder.py -name lirik -t vod -v 13245678
Repairing recorded folder:
recorder.py -name lirik -t repair
```
