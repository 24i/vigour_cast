# Vigour Cast
Cordova Plugin to discover and communicate with Cast type devices

| Device | Custom Receiver | Direct Video Stream |
| --- | --- | --- |
| Chromecast | yes | no |
| Airplay | no | yes |

## JavaScript API

exposes `window.vigour.cast`
___
### window.vigour.cast

#### Methods

##### cast.startScanning()

##### cast.stopScanning()

#### Events

##### deviceFound
passes `device`
##### deviceLeft
passes `device`
##### deviceUpdate
passes `device`
___
### device

#### Methods

##### connect

##### disconnect

##### openApp(obj)
`obj` is platform specific

success callback is passed `session`

##### play()

##### pause()

##### seek(ratio)

##### volume(ratio)

___
### session

#### Methods

##### openChannel(obj)
`obj` is platform specific, for ChromeCast, it needs the `namespace` property.


