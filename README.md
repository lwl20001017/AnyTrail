# AnyTrail
Create any shape of trail under player and generate RT
-  Code by pure compute shader
- Support fluid / trail / wave / patterns
- Trail will be drawn on a canvas moving with player(refreshing in realtime), so you can draw more detail within screen and erase trails outside screen
- Can be used to 
    - Draw 2D fluid/wave on the surface of water, and use the RT as bumpmap to water
    - Draw trail of any shape of footprints(by customizing pattern) on sand/snow

# Use
- Attach `AnyTrailCanvas.cs` on center gameobject and open effect in inspector
- Attach `FluidWriter.cs` / `PatternWriter.cs` / `TrailWriter.cs` / `WaveWriter.cs` on drawer gameobject(can be same with center gameobject), and open drawer in inspector panel
- Include `AnyTrailShaderInclude.hlsl` in shader and use `SampleAnyTrailXXX()` function to sample the result RT based on `positionWS.xz`


# AnyTrail Playground
- Download the `.exe` file from github release and run 😊
- **WSAD to move, SPACE button to draw, 1234 to open/close different drawers**

# Demo
[![](https://i.ytimg.com/vi/e34BJWlViKs/maxresdefault.jpg)](https://youtu.be/e34BJWlViKs "")