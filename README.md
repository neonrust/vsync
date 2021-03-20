# vsync

Video service helper script.

## Video services supported

- YouTube
- Twitch

## Features

Generallt, it list videos in a playlist or channel/user.

    vsync <source> <options>
    vsync <video url>          # a bit pointless, however
    vsync <playlist url>
    vsync <service>:<account>

Where <options> might be:

  -n N              Top N videos
  
  <any string>      Match title
  
  <absolute path>   Download videos to local directory.  Absolute path
                    is used to make it possible to distinguish from
                    <any string> variant.

Some examples:

    vsync youtube:nasa 'mars rover'
    vsync https://www.youtube.com/playlist?list=PL2aBZuCeDwlTxZeGRlKrWpLiX_W7jpt6p
    vsync twitch:suddendeathtv 2on2 /home/user/Videos


## Dependencies

- youtube-dl
- ptyprocess
