# vanta-maptiles

GTA V map tiles for the Vanta resources (vanta_mdt, vanta_policejob, vanta_blackmarket, vanta_spawn), served through jsDelivr so no resource has to ship its own copy:

```
https://cdn.jsdelivr.net/gh/VantaScripts5/vanta-maptiles@v1/{style}/{z}/{x}/{y}.webp
```

| Style | Folder |
|---|---|
| Satellite | `satellite/` |
| Atlas | `atlas/` |
| Grid | `grid/` |

Zoom levels 0-5, 256 px WebP tiles. Coordinates follow the calibrated CRS from [RiceaRaul/gta-v-map-leaflet](https://github.com/RiceaRaul/gta-v-map-leaflet).

## Versions

Resources point at a tag (`@v1`), so a release never changes under a running server. To change tiles, commit and push a new tag (`v2`) and update `Config.Map.tiles` (or `Config.MapTiles`) in the resources.

## Self-hosting

Any web server or other resource can serve the same folders. Point the resource's tile setting at its base URL, for example `https://cfx-nui-my_tiles/tiles`.

The map imagery is from Grand Theft Auto V, © Rockstar Games.
