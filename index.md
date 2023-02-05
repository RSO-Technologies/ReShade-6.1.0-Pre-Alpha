# ReShade 6.1
## Advanced post-processing everywhere.

ReShade is a generic post-processing injector for games and video software developed by crosire. Imagine your favorite game with ambient occlusion, real depth of field effects, color correction and more ... ReShade exposes an automated and generic way to access both frame color and depth information (latter is automatically disabled during multiplayer to prevent exploitation) and all the tools to make it happen.

The possibilities are endless! Add advanced depth-edge-detection-driven SMAA antialiasing, screen space ambient occlusion, depth of field effects, chromatic aberration, dynamic film grain, automatic saturation and color correction, cross processing, multi-pass blurring ... you name it.

`ReShade supports all of Direct3D 9, Direct3D 10, Direct3D 11, Direct3D 12, OpenGL and Vulkan.
A computer with Windows 7 SP1, 8.1, 10 or 11 and .NET Framework 4.6.2 or higher installed is required.`

ReShade features its very **own shading language** and **compiler**, called ReShade FX. The syntax is based on HLSL, adding useful features designed for developing post-processing effects: Define and use textures right from the shader code, render to them, change renderstates, retrieve color and depth data, request custom values like timers or key states, ...

And that's not it. Write your shaders just once, they'll work **everywhere**, regardless of your target being Direct3D or OpenGL: ReShade takes care of compiling them to the right shader model and language (HLSL, GLSL or SPIR-V).

ReShade 5.0 introduced a powerful add-on API that makes it possible to write add-ons for both ReShade and the games it is used with. For more information check out the documentation.

## Open Source

As of January 1st 2017, ReShade is **open sourced** under the terms and conditions of the BSD 3-clause license! You can help development with your own contributions via the [official GitHub repository](https://github.com/crosire/reshade).

## Download
Pre-Alpha Version 6.1.0 was released on January 15th 2023.

**Use preset files (*.ini) that can be created from ReShade's in-game user interface to share your configurations.
Do NOT share the binaries or shader files. Link users to this website instead.**

[![data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGcAAAAnCAYAAAASGVaVAAAAAXNSR0IArs4c6QAABUVJREFUaEPtm39I1Gccx1/njxRvaol3ZnRYcZI0o02bUSlDOLKByzlhbTU2ttZYbUQNRvtFY2ODNUaarMZYP6U12lCzyaw4FitXFBW2JAqlFjrP+eM6c2d33n298b0f5Z2VdTyjr/Dcn1++z+d5P+/X83k+n+cLp9v81VZf/NU0dN1JoOiQv0frwEiMgsf4LzGPu9FteavGp/v7sUerSM4e5oBnZBh3hgNdZXmtD6/MGC3tD8WnMODpQ1f5bJ1PS8KkFhjxKdy4JeFoci9IOJrEEhAl4Ug4GnZAw9Jk5kg4GnZAw9Jk5kg4GnZAw9Jk5kg42nAg/4tSiubGY7fWU1P9f2rKpuLHXEz6QVqXWbFGOZXAzAkJGqVEUXD3D9B28ALWRkeUEsUNk3D04LYN4hwG9EmkpccCCnbraWqq/xHndBSRJBy9h46djdQ2BNwzLi+kYqWBBGWQ1k+tWFuicFXQEAknAg4kUVxVwrxZMPBHM7s396I+y1mVx0KLgVR9wHl3n4NrP5/mcNMQWBayet1U9D1d1L5xmg4g5+NnWFqQSE9DPft3qiPmsPyn2WTGOzhXfoyE7eXkTvfQc8pBwpMGUhPVhPVgP36Jg5VXuQmMhTOODr+yJOZtWEBBwWT0Qa3ePgftIa3qK+bZlL2fzUxjfGAt13txphtI017NCc8cVWzKhiW8XqyHq21UrW/F9LaFspJk4hQPA50ulNh4UqYnEqe4aN/WRKM1sqCaKNs7n5lTuB2D4oWs3jAVfed1dq09T4EfTgBIWEycXN50lMMtY+GMrwNM6yxUWJLB6aSjxY43w4DJnEicy87JF37nDFmU7c0LaHM6sfeNEJueHNx0mmsIxsJhnYX16gI7r1O1tj+4GA8de36jtm7Iv9tmbFzCc4vvACz4chmL5oDtwCEOdAVBKOqbgUz5a+MSKhbrGTjezO6ve7H44Sj01FnZv0eNmcTS70rIyQT7kXpqtkXCCZl6fx05K/OYYYzh5sWznPS3XQZKdxRiNgbXSSFrVhlIcPZy4t1mztmAzFxWbM3GmDgB4IRnziReOZRFmrqYl5o5F6onoUy42cuxl5u5sPJp3lmehtJygUanmYrF0G71YLYk+4F1PVVO/iwn7ZuO0thCEE74xggA43brHH6s5T2YDjIo+mQuuXOTSZg0uvgF58oKbDzvlSt8896l4AuabaUjMyey5pjubkppIWveNJAQgkMuK+qzMfZ3c42pzIzv5vCrg+TVZ5PW3oVt+jRMw+qzU1xGIJwIHXHBu5HX1s35XzqxO8H84nzMmeFw3Bdb+fajtokFZ2y3FtpV9z9O1GPJsr0kUEfU4/zMWb7/vIOiqnLys4BYGG1IIEseJnMeRMcQFfvmYUpRtTZSW6cqyaB01yLM6RPyWBv/nnPPQoyLa9VNNASv1KZgXUF9XtlEwzFgVTHryyb7707+evRDAN7Dw+HejckoHUVblpFvjr1T7Kckk5qizhjaCBmU7liE2TghGoJR57L6hcBmp+3X1ogvBA/SwgJPLOC1z6aReuPO8UXouAs2BieC00UDZ9yWXo2dOYulH84hJyvQJnt7erEpBkxqo2E9Qk310F1a6Q56JpkwZWqmIRB0U5Rhbjsg8NuadFW0AxKOaEcFxpNwBJopOpSEI9pRgfEkHIFmig4l4Yh2VGA8CUegmaJDSTiiHRUYT8IRaKboUBKOaEcFxpNwBJopOpQy4sXh6kdX9Xytz+eRfzsUbXC08dSsueUZwuVzotv9wUFf/5/D6HQSULSGihin/vdzZERhWHHj8g6RkBXDf6SPTwnG3gcGAAAAAElFTkSuQmCC]][https://google.com/]


*Digital Signature Thumbprint: 5896E526457FB832454465745656F50ACD47C49F*
