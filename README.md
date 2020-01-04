![raspi-3dtouch](https://user-images.githubusercontent.com/11918596/71766147-2a298d00-2f40-11ea-8f04-33c2ce08d0b7.png)

# threedtouch
control 3dtouch with python on raspberry pi

# Usage

## start pigpiod
```
$ sudo pigpiod
```

## Push-pin Down
```
import threedtouch

threedt = threedtouch.ThreeDTouch(gpio_hw_pwm=18, gpio_sw=23)
threedt.pp_down()
```

## Push-pin Up
```
threedt.pp_up()
```

## Self-test
```
threedt.test()
```

## Alarm Release
```
threedt.alarm_release()
```

## wait for the Push-pin to be touched
```
threedt.wait_touched()
```
