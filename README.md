## Development

### Adding 3rd Person Controller

Supply the animator as needed: e.g. [`astronautA.controller`](Assets/StarterAssets/ThirdPersonController/Character/Animations/astronautA.controller)

FBX model:

- Go to Animations -> Choose an animation -> Events -> add the events needed

Player Game Object:

- Add 'Empty' called PlayerCameraRoot (adjust transform as needed)
- Make sure the Layer is other than "Default", so `ThirdPersonController.cs : GroundedCheck()` sphere wouldn't constantly collide with it.
- Add Audio Files to **Landing Audio Clip** and **Footstep Audio Clips**

PlayerFollowCamera Game Object:

- Set 'Follow' to PlayerCameraRoot

Third Pesron Controller (Script)

- Set 'Ground Layers' to Default so `ThirdPersonController.cs : GroundedCheck()` will set the correct LayerMask
- Set 'Cinemachine Camera Target' to PlayerCameraRoot

In **StarterAssetsInputs.cs** and **ThirdPersonController.cs**:

- Comment `#if ... // && STARTER_ASSETS_PACKAGES_CHECKED`

### Enabling Universal Render Pipepline (URP)

[![](https://img.youtube.com/vi/m6YqTrwjpP0/0.jpg)](https://www.youtube.com/watch?v=m6YqTrwjpP0)

[![](https://img.youtube.com/vi/9tjYz6Ab0oc/0.jpg)](https://www.youtube.com/watch?v=9tjYz6Ab0oc)
