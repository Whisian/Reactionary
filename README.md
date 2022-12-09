# Reaction Test.

## *OBJECTIVE*
In this test there is a countdown, and when the countdown ends the player must press the button as fast as they can
when the button is pressed, the players time will show up and a song will play.

## PSEUDO CODE
- Countdown will start when microbit is shaked
- Pressing button A will be registered after the countdown is over
- After input is registered, time will display and song will play

## REQUIRED OBJECTS
- 1 Microbit
- 1 9V Battery
- 1 Buzzer

## CODE
input.onButtonPressed(Button.A, function () {
    led.stopAnimation()
    basic.showNumber(input.runningTime())
    for (let index = 0; index < 1; index++) {
        music.changeTempoBy(20)
        music.playTone(247, music.beat(BeatFraction.Whole))
        music.playTone(330, music.beat(BeatFraction.Whole))
        music.playTone(330, music.beat(BeatFraction.Half))
        music.playTone(392, music.beat(BeatFraction.Half))
        music.playTone(370, music.beat(BeatFraction.Whole))
        music.playTone(330, music.beat(BeatFraction.Double))
        music.playTone(494, music.beat(BeatFraction.Whole))
        music.playTone(440, music.beat(BeatFraction.Double))
        music.playTone(440, music.beat(BeatFraction.Whole))
        music.playTone(370, music.beat(BeatFraction.Double))
        music.playTone(370, music.beat(BeatFraction.Whole))
        music.playTone(330, music.beat(BeatFraction.Whole))
        music.playTone(330, music.beat(BeatFraction.Half))
        music.playTone(392, music.beat(BeatFraction.Half))
        music.playTone(370, music.beat(BeatFraction.Whole))
        music.playTone(311, music.beat(BeatFraction.Whole))
        music.playTone(311, music.beat(BeatFraction.Whole))
        music.playTone(349, music.beat(BeatFraction.Whole))
        music.playTone(247, music.beat(BeatFraction.Double))
        music.playTone(247, music.beat(BeatFraction.Whole))
        music.playTone(330, music.beat(BeatFraction.Whole))
        music.playTone(330, music.beat(BeatFraction.Half))
        music.playTone(392, music.beat(BeatFraction.Half))
        music.playTone(370, music.beat(BeatFraction.Whole))
        music.playTone(330, music.beat(BeatFraction.Double))
        music.playTone(494, music.beat(BeatFraction.Whole))
        music.playTone(587, music.beat(BeatFraction.Double))
        music.playTone(554, music.beat(BeatFraction.Whole))
        music.playTone(523, music.beat(BeatFraction.Double))
        music.playTone(415, music.beat(BeatFraction.Whole))
        music.playTone(523, music.beat(BeatFraction.Whole))
        music.playTone(523, music.beat(BeatFraction.Half))
        music.playTone(494, music.beat(BeatFraction.Half))
        music.playTone(466, music.beat(BeatFraction.Whole))
        music.playTone(233, music.beat(BeatFraction.Double))
        music.playTone(392, music.beat(BeatFraction.Whole))
        music.playTone(330, music.beat(BeatFraction.Double))
    }
})
input.onGesture(Gesture.Shake, function () {
    basic.showNumber(3)
    control.waitMicros(1)
    basic.showNumber(2)
    control.waitMicros(1)
    basic.showNumber(1)
    control.waitMicros(0)
    basic.clearScreen()
})
