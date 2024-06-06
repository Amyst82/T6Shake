
# T6Shake

BO2 Camera shake mod made for Dmitry Norton. The mod also supports camera roll and fov interpolation.


## Installation

Add BO2Shake.Red32n to your Redacted plugins folder.

```bash
  ...\Redacted\Plugins
```
    
## Dvars

#### T6Shake has some custom dvars (console commands) that can help you to operate the mod.

| Dvar name | Default value | Min value | Max value |                       Description             |   Type  | 
| :-------- | :------------ | :-------- |:--------- | :-------------------------------------------- | :------ |
| `c_Shake` |        0      |      0    |      1    |  `Determines if the camera uses shake effect.`|  `Bool` |
| `c_ShakeSpeed` |        1.0      |      0.0    |      10.0    |  `Speed of camera shake.`|  `Float` |
| `c_ShakeAmount` |       1.0      |      0.0    |      10.0     |  `Overall amount of camera shake.`|  `Float` |
| `c_ShakePosition *` |        1.0      |      0.001    |      1000.0    |  `Intensity of camera position shake.`|  `Float` |
| `c_ShakeRotation` |        1.0      |      0.001    |      1000.0    |  `Intensity of camera rotation shake.`|  `Float` |
| `c_FreeRoamSpeed` |        1.0      |      0.0    |      10.0    |  `Speed of free roam camera.`|  `Float` |
| `c_RollStep` |        5.0      |      0.0    |      90.0    |  `Amount that camera roll angle will be increased/decreased by during mouse wheel scrolling.`|  `Float` |
| `c_ShowMarkerDebug` |        1      |      0    |      1    |  `Determines if the camera marker info (roll and fov) is displayed.`|  `Bool` |

##### * - Not implemented yet.
#### The dvar list will be extended.

## Usage

#### T6Shake takes information of camera control points (markers) from game memory. No other tools needed. Camera roll and fov are also stored in a marker structure. 

### Operating camera shake through dvars
```bash
  Enter commands listed above with a parameter in any BO2 Console.
```
### Set camera marker roll
```bash
  Simply scroll down/up your mouse wheel while Edit Camera Mode (where you place markers). Roll value will be automatically attached to a marker that is gonna be added.
```
### Set camera marker fov
```bash
  Simply scroll down/up your mouse wheel with Left Control key pressed while Edit Camera Mode (where you place markers). Roll value will be aumatically attached to a marker that is gonna be added.
```
### Edit camera marker fov/roll
```bash
  Enter camera marker repositioning mode and change Fov/Roll.
```
### Camera usage
```bash
  The new interpolated camera (with shake effect and roll/fov) updates every time you enter DollyCamera mode. To get updated roll and fov values be in your camera just simple re-enter DollyCamera mode. Shake effect updates automatically.
```
## Acknowledgements

 - [Video tutorial how to (coming soon)]()
 - [BO2 Console V4](https://discord.com/channels/453934547151749130/869568094807392297/869574048991051787)
 - [Old Advanced Dolly Cam Mod](https://airyz.xyz/p/t6-advanced-dolly/)

