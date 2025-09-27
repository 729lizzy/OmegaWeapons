A client-side mod that fixes DMR reloading to 11 instead of 12 when there is 1 bullet left in clip.

Requires Bepinex, but is not dependent on `GTFO-API` plugin, so you can remove `GTFO-API.dll` from `plugins` folder to keep vanilla rundown and progression.

============ Change Log ============

v0.0.6
- Made methods public for mods that patch reload, since double reloading can cause conflicts

v0.0.5
- Fixed guns not being given full clip on drop

v0.0.4
- Avoid all issues by simply performing the reload twice internally. (If the first reload gets you max clip - 1, the second will fix it)

v0.0.3
- Added sanity checks for ammo in reserve falling below 0, ammo in clip gained not matching ammo in reserve lost and clip exceeding maximum clip size to try and avoid bugged cases.

v0.0.2
- Fixed a bug where some guns would magically be given an extra bullet from thin air

v0.0.1
- Initial Release