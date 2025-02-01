# beep-MICROBIT
beep!
## Yell into your microbit (V2 ONLY) and it will play music for you!
## COPY PASTE INTO ```https://makecode.microbit.org/#editor```

## PYTHON
```def on_sound_loud():
    music.play(music.string_playable("B A G A G F A C5 ", 300),
        music.PlaybackMode.UNTIL_DONE)
input.on_sound(DetectedSound.LOUD, on_sound_loud)

music.play(music.tone_playable(262, music.beat(BeatFraction.WHOLE)),
    music.PlaybackMode.UNTIL_DONE)
music.stop_all_sounds()

def on_forever():
    basic.show_string("Scanning...")
basic.forever(on_forever)

def on_in_background():
    datalogger.log(datalogger.create_cv("", 0),
        datalogger.create_cv("", 0),
        datalogger.create_cv("", 0),
        datalogger.create_cv("", 0),
        datalogger.create_cv("", 0),
        datalogger.create_cv("", 0),
        datalogger.create_cv("", 0))
control.in_background(on_in_background)
```
## JAVASCRIPT
```
input.onSound(DetectedSound.Loud, function on_sound_loud() {
    music.play(music.stringPlayable("B A G A G F A C5 ", 300), music.PlaybackMode.UntilDone)
})
music.play(music.tonePlayable(262, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
music.stopAllSounds()
basic.forever(function on_forever() {
    basic.showString("Scanning...")
})
control.inBackground(function on_in_background() {
    datalogger.log(datalogger.createCV("", 0), datalogger.createCV("", 0), datalogger.createCV("", 0), datalogger.createCV("", 0), datalogger.createCV("", 0), datalogger.createCV("", 0), datalogger.createCV("", 0))
})
```
