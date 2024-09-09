# splat_shop // nerf_cinematography 

A WebGL implementation real time renderer 3D Gaussian Splat viewer with brush and eraser tool, color burn and dodge effects, camera settings adjusters, screenshots and VR mode. 

currently implementing drag and drop of second splat on top of the first, quite difficult at the moment.

Based on the [splat](https://github.com/antimatter15/splat) viewer by [antimatter15](https://github.com/antimatter15).

# features

3D Navigation: Use mouse, keyboard, touch, or oculus controls to move around the 3D space.
Camera Controls: Adjust exposure, focal length, and aperture to change the visual appearance of the scene.
Editing Tools:

Brush: Paint splats with a chosen color
Eraser: Remove color from splats
Dodge: Lighten splats
Burn: Darken splats


Undo Functionality: Revert recent changes to the scene.
Screenshot Tool: Capture and save the current view as a PNG image.
VR Support: Enter immersive VR mode for supported devices.
File Support: Load .splat and .ply files, as well as camera configuration JSON files.


## controls

movement (wasd)

- a/d arrow keys to strafe side to side
- w/s arrow keys to move forward/back
- `space` to jump

camera angle (arrows)

- `left`/`right` to turn camera left/right
- `up`/`down` to tilt camera up/down
- `q`/`e` to roll camera counterclockwise/clockwise
- `i`/`k` and `j`/`l` to orbit

trackpad
- scroll up/down to orbit down
- scroll left/right to orbit left/right
- pinch to move forward/back
- ctrl key + scroll up/down to move forward/back
- shift + scroll up/down to move up/down
- shift + scroll left/right to strafe side to side

mouse
- click and drag to orbit
- right click (or ctrl/cmd key) and drag up/down to move forward/back
- right click (or ctrl/cmd key) and drag left/right to strafe side to side

touch (mobile)
- one finger to orbit
- two finger pinch to move forward/back
- two finger rotate to rotate camera clockwise/counterclockwise
- two finger pan to move side-to-side and up-down

other
- press 0-9 to switch to one of the pre-loaded camera views
- press '-' or '+'key to cycle loaded cameras
- press `p` to resume default animation
- drag and drop .ply file to convert to .splat
- drag and drop cameras.json to load cameras

## other features

- press 'b' to enable brush tool
- press 'z' to enable eraser tool
- press 'v' for cursor
- press 'n' to enable dodge tool
- press 'm' to enable color burn tool
- open custom `.splat` files by adding a `url` param to a CORS-enabled URL
- drag and drop a `.ply` file which has been processed with the 3d gaussian splatting software onto the page and it will automatically convert the file to the `.splat` format