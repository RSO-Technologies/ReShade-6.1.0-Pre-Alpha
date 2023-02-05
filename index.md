# ReShade 6.1
## Advanced post-processing everywhere.

ReShade is a generic post-processing injector for games and video software developed by crosire. Imagine your favorite game with ambient occlusion, real depth of field effects, color correction and more ... ReShade exposes an automated and generic way to access both frame color and depth information (latter is automatically disabled during multiplayer to prevent exploitation) and all the tools to make it happen.

The possibilities are endless! Add advanced depth-edge-detection-driven SMAA antialiasing, screen space ambient occlusion, depth of field effects, chromatic aberration, dynamic film grain, automatic saturation and color correction, cross processing, multi-pass blurring ... you name it.

###ReShade supports all of Direct3D 9, Direct3D 10, Direct3D 11, Direct3D 12, OpenGL and Vulkan.
###A computer with Windows 7 SP1, 8.1, 10 or 11 and .NET Framework 4.6.2 or higher installed is required.

ReShade features its very **own shading language** and **compiler**, called ReShade FX. The syntax is based on HLSL, adding useful features designed for developing post-processing effects: Define and use textures right from the shader code, render to them, change renderstates, retrieve color and depth data, request custom values like timers or key states, ...

And that's not it. Write your shaders just once, they'll work **everywhere**, regardless of your target being Direct3D or OpenGL: ReShade takes care of compiling them to the right shader model and language (HLSL, GLSL or SPIR-V).

ReShade 5.0 introduced a powerful add-on API that makes it possible to write add-ons for both ReShade and the games it is used with. For more information check out the documentation.

## Open Source

As of January 1st 2017, ReShade is **open sourced** under the terms and conditions of the BSD 3-clause license! You can help development with your own contributions via the [official GitHub repository](https://github.com/crosire/reshade).

## Download
Pre-Alpha Version 6.1.0 was released on January 15th 2023.

**Use preset files (*.ini) that can be created from ReShade's in-game user interface to share your configurations.
Do NOT share the binaries or shader files. Link users to this website instead.**

<kbd> <br> Title <br> </kbd>[https://github.com/MarkedDown/Buttons/blob/main/Types/KBD.md]

*Digital Signature Thumbprint: 5896E526457FB832454465745656F50ACD47C49F*
