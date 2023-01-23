### @activities true
### @explicitHints true

# ERPS STEM WEEK :: Traffic Lights - Basic Tutorial

## Introduction
### Introduction Step @unplugged
In this tutorial, you will start by getting all of the lights to come on!
![All lights lit up](https://raw.githubusercontent.com/niaxotim/erps-stem-week-2023/master/assets/traffic_lights_basic.png)


### Assembly
The traffic light has 3 different LED bulbs, each of which can be controlled individually.
But we are going to start nice and simple! Can you make all 3 lights come on
at the same time?  First, make sure your micro:bit is connected to your lights.

## Traffic Lights
### Step 1

First we need to add some input. We will create code to turn all the lights on and off with buttons presses.  
Add ``||input:on Button A||``.

#### ~ tutorialhint
```blocks
input.onButtonPressed(Button.A, function () {
	
})
```

### Step 2

From the STOP:bit blocks, add into the ``||input:on Button A||`` block 3 x ``||Kitronik_STOPbit.Turn Traffic Light On||`` blocks.

#### ~ tutorialhint
```blocks
input.onButtonPressed(Button.A, function () {
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Red, Kitronik_STOPbit.DisplayLights.On)
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Red, Kitronik_STOPbit.DisplayLights.On)
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Red, Kitronik_STOPbit.DisplayLights.On)
})
```

### Step 3
Notice all of the blocks have the colour "Red" selected.  Change one block to "Yellow" and another to "Green".
#### ~ tutorialhint
```blocks
input.onButtonPressed(Button.A, function () {
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Red, Kitronik_STOPbit.DisplayLights.On)
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Yellow, Kitronik_STOPbit.DisplayLights.On)
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Green, Kitronik_STOPbit.DisplayLights.On)
})
```

### Step 4
This code will turn on all the LEDs when ``||input:Button A||`` is pressed. See if you can create the similar code to turn the LEDs off when ``||input:Button B||`` is pressed.
#### ~ tutorialhint
```blocks
input.onButtonPressed(Button.A, function () {
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Red, Kitronik_STOPbit.DisplayLights.On)
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Yellow, Kitronik_STOPbit.DisplayLights.On)
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Green, Kitronik_STOPbit.DisplayLights.On)
})
input.onButtonPressed(Button.B, function () {
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Red, Kitronik_STOPbit.DisplayLights.Off)
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Yellow, Kitronik_STOPbit.DisplayLights.Off)
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Green, Kitronik_STOPbit.DisplayLights.Off)
})
```

### Step 5
Connect your BBC micro:bit and click ``|Download|``. Once programmed, power the BBC micro:bit and press ``||input:buttons A and B||`` to turn the lights On and Off.
