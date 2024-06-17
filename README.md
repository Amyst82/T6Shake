![changing roll and fov](https://github.com/Amyst82/T6Shake/assets/20230176/b1737e27-3fd6-41f6-a23f-50cb8dfb8727)
# T6Shake
*Somehow i ended up with this working title xd*

## BO2 Camera shake mod made for Dmitry Norton. The mod also supports frozen camera mode with roll and fov interpolation.


## Installation

Add BO2Shake.Red32n to your Redacted plugins folder.

```bash
  ...\Redacted\Plugins
```
    
## Dvars

#### T6Shake has some custom dvars (console commands) that can help you to operate the mod.

| Dvar name | Default value | Min value | Max value |                       Description             |   Type  | 
| :-------- | :------------ | :-------- |:--------- | :-------------------------------------------- | :------ |
| `c_shake` |        0      |      0    |      1    |  *Determines if the camera uses shake effect.*|  `Bool` |
| `c_shakeSpeed` |        1.0      |      0.0    |      10.0    |  *Speed of camera shake.*|  `Float` |
| `c_shakeAmount` |       1.0      |      0.0    |      10.0     |  *Overall amount of camera shake.*|  `Float` |
| `c_shakePosition` |        1.0      |      0.001    |      1000.0    |  *Intensity of camera position shake.*|  `Float` |
| `c_shakeRotation` |        1.0      |      0.001    |      1000.0    |  *Intensity of camera rotation shake.*|  `Float` |
| `c_freeRoamSpeed` |        1.0      |      0.0    |      10.0    |  *Speed of free roam camera.*|  `Float` |
| `c_rollStep` |        5.0      |      0.0    |      90.0    |  *Amount that camera roll angle will be increased/decreased by during mouse wheel scrolling.*|  `Float` |
| `c_showMarkerDebug` |        1      |      0    |      1    |  *Determines if the camera marker info (roll and fov) is displayed.*|  `Bool` |
| `c_frozen` |        0      |      0    |      1    |  *Determines if the frozen camera mode is turned on.*|  `Bool` |
| `c_demoTimescaleStep` |        1.0      |      0.0    |      10.0    |  *Step the demo timescale will be changed with*|  `Float` |

#### The dvar list will be extended.

## Usage

#### T6Shake takes information of camera control points (markers) from game memory. No other tools needed. Camera roll and fov are also stored in a marker structure. 

### Operating camera shake through dvars
```
  Enter commands listed above with a parameter in any BO2 Console.
```
### Set camera marker roll
Simply `scroll down/up your mouse wheel` while `Edit Camera Mode` (where you place markers). Roll value will be automatically attached to a marker that is gonna be added.
### Set camera marker fov
Simply `scroll down/up your mouse wheel` with `Left Control key` pressed while `Edit Camera Mode` (where you place **markers**). Roll value will be aumatically attached to a marker that is gonna be added.

![](https://s12.gifyu.com/images/Srbuh.gif)

### Changing demo timescale step
You can change your demo timescale step using `c_demoTimescaleStep` dvar. In the GIF below the dvar is set to `0.05`.

![](https://s12.gifyu.com/images/Srbug.gif)
### Rotation shake
Rotation shake can be applied with `c_shake 1` command and `c_shakeRotation` command set above zero. 

![](https://s10.gifyu.com/images/SrbuY.gif)
### Position shake
Position shake can be applied with `c_shake 1` command and `c_shakePosition` command set above zero. 

![](https://s12.gifyu.com/images/Srbuo.gif)
#### You can combine position shake and rotation shake together.

![](https://s10.gifyu.com/images/Srbu1.gif)

### Changing roll step
Amount the roll will be increased/decreased with your mouse wheel scrolling can be also changing with `c_rollStep` command.

![](https://s10.gifyu.com/images/SrbQ3.gif)

### Camera marker info
You can show or hide camera marker info (containing roll and fov) with `c_showMarkerDebug` command.

![](https://s10.gifyu.com/images/SrbuX.gif)

### Free camera/edit camera mode speed
Speed of your camera can be changed with `c_freeRoamSpeed` command or you can increase the speed by pressing `+ (plus)` key and decrease speed with `- (minus)` key.

![](https://s12.gifyu.com/images/SrbQS.gif)

### Edit camera marker fov/roll
Enter camera marker `repositioning mode` and change Fov/Roll.
### Camera usage
The new interpolated camera (with shake effect and roll/fov) updates every time you `enter DollyCamera mode`. To get `updated roll and fov values be in your camera` just simple re-enter DollyCamera mode. Shake effect **updates automatically**.

![](https://s10.gifyu.com/images/SrbQp.gif)

### Frozen Camera usage
Frozen camera mode can be turned on using `c_frozen 1` command. Simply press the play button with already set markers or just add new ones while you demo is stopped. Frozen camera supports shake and roll/fov interpolation as well.

![](https://s10.gifyu.com/images/SrbQu.gif)

## Useful links

 - [Video tutorial how to (coming soon)]()
 - [BO2 Console V4](https://discord.com/channels/453934547151749130/869568094807392297/869574048991051787)
 - [Old Advanced Dolly Cam Mod](https://airyz.xyz/p/t6-advanced-dolly/)

