# DF Smooth Movement

> [!NOTE]
> We will use this project to keep adding crazy and experimental visual features.<br/> If you want a vanilla experience use DFHack's smooth-movement.

A visual plugin for Dwarf Fortress that makes movement smoother.

## Features

- **Smooth movement:** creatures, hauled items, and vehicles glide between tiles.
- **Synced icons:** status icons follow their creature while it moves.
- **Animated carts:** wheelbarrows and minecarts move smoothly too.
- **Sprites flip** creatures can optionally face the direction they are walking.
- **Free camera:** the camera can optionally glide and be dragged with the mouse (WIP).
- **Adventure mode tuning:** in adventure mode the camera glide switches on and steps ease linearly, so walking and running read as one steady motion.

## Installation

1. Download the release archive for your operating system and DFHack version.
2. Extract it into the Dwarf Fortress/DFHack folder.
3. Check that the plugin is in one of these locations:
   - Linux: `hack/plugins/smooth-movement.plug.so`
   - Windows: `hack/plugins/smooth-movement.plug.dll`
4. Start Dwarf Fortress through DFHack and run this in the console:

```text
load smooth-movement
enable smooth-movement
```

## Useful commands

```text
smooth-movement             # show plugin status
disable smooth-movement     # disable the plugin
smooth-movement flip on     # enable sprites flip
smooth-movement camera on   # enable the free camera
smooth-movement speed 80    # milliseconds per tile step (20-500, default 100)
smooth-movement ease linear # linear or smooth (smoothstep, the default outside adventure mode)
smooth-movement adventure off # turn the adventure mode tuning off (default on)
```

## Compatibility

Requires DFHack 53.16-r1.1 and the SDL 2D renderer. Always download the plugin version that matches your DFHack version.

## License

MIT. See [LICENSE](LICENSE).
