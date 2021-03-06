**v0.7.3**

- Fix glitch in the npm release of `v0.7.2`.

**v0.7.2**

- Provide proper ESM instead of pointing to the source code.

**v0.7.1**

- Replaced `hover` event with `pointover` and `pointout` to be able to know when a point is not hovered anymore.

**v0.7.0**

- Allow changing the lasso smoothness via `set({ lassoMinDelay, lassoMinDist })` where `lassoMinDelay` is the minimum number of milliseconds between mousemove events before the lasso is extended and `lassoMinDist` is the minimum number of pixels the mouse has to move.

**v0.6.0**

- Simplify API: `style()`, `attr()`, `scatterplot.canvas`, `scatterplot.regl`, and `scatterplot.version` are merged into `get()` and `set()`. The function signature is identical to `style()` and `attr()` so all you have to do is rename.
- Add recticle. It's not shown by default but can be activated with `set({ showRecticle, recticleColor })`.
- Fix a regression that caused interrupted panning

**v0.5.1**

- Fix a bug in categorical color encoding

**v0.5.0**

- Set default aspect ratio to 1. It can be changed via `attr({ aspectRatio })`
- Add property to set `lassoColor` via `style({ lassoColor })`
- Expose helper (`createTextureFromUrl`) for creating a texture from an image URL
- Expose regl instance via `scatterplot.regl`
- Replace `mouse-position` and `mouse-pressed` with internal code
- Avoid click selections upon mousedown + mousemove + mouseup
- Add tests for all public API endpoints
- Fix several smaller bugs

**v0.4.0**

- Use a combination of linear and log2 scaling for point size
- Add support for background images
- Add API documentation
- Switch to single quotes
- Export version

**v0.3.3**

- Add endpoint for changing the background color
- Allow setting view on initialization
- Remove event listeners on `destroy()`
- Rename `camera` event to `view` and publish the view matrix
- Fix issues with setting colors
- Fix resetting view

**v0.3.2**

- Update third party libraries
- Switch to browser-based tests
- Set more strict linting

**v0.3.1**

- Fix nasty floating point issue when working with large textures (> 100.000 points)
- Make point size dependent on zoom level

**v0.3.0**

- Optimize rendering: up to about 500K points render fine. Usable for up to 1M points.
- Add support for one categories and one value per point for color encoding.
- Add visual outline for selected points for better highlighting.
- Add test setup and some base tests.
- Many bug fixes and under the hood improvements.

**v0.2.0**

- Add fast lasso selection
- Support rotations

**v0.1.0**

- Initial working version. **Warning:** this version is not optimized yet and only works fluidly for up to 50.000 points.
