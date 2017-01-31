# Pulse audio equalizer presets

This is the Boosted and Perfect EQ from [here](http://www.ziyadnazem.com/post/956431457/the-perfect-eq-settings-unmasking-the-eq).

## Installation

Put the preset files in the pulse folder.

- Ubuntu: `~/.config/pulse/presets/`

- Fedora: `~/.pulse/presets/`

## Hot tip
If you want to improve the sound quality and are using PulseAudio, check this out:

- Edit the file called `/etc/pulse/daemon.conf`
- Add this config:
```
    resample-method = src-sinc-best-quality
    default-sample-format = s24le
    default-sample-rate = 96000
```
- Reset pulseaudio typing `pulseaudio -k && pulseaudio --start`
- Enjoy :)

For more information, like medium quality config and etc, see:
[How To: Enable High Quality Audio in Linux](http://r3dux.org/2013/12/how-to-enable-high-quality-audio-in-linux/)
