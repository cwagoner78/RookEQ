# Rook EQ: quick start and controls

This guide covers the development version of Rook EQ. Controls may change before release.

## Getting started

Rook EQ runs in a 64-bit Windows DAW that supports VST3 plugins. If you have received a test build, follow its installation instructions and rescan your DAW's plugin list.

1. Insert Rook EQ on an audio track or bus.
2. Play the section you want to work on.
3. Click an empty area of the graph to add a band. Rook EQ starts with no active bands.
4. Drag the band's node horizontally to set frequency. For bell and shelf filters, drag vertically to set gain.
5. Use the selected band's controls below the graph for exact values and filter shape.
6. Compare with bypass and adjust the output trim as needed.

## Bands and filters

Rook EQ provides up to 12 bands. Select a node to show its controls. The available controls follow the selected filter type.

| Filter | Use |
|---|---|
| Bell | Boost or cut around a selected frequency. |
| Low shelf / High shelf | Adjust the low or high end over a broad range. |
| Tilt shelf | Shift the balance between lows and highs. |
| Notch | Reject a narrow frequency region. |
| Band-pass | Keep a region while attenuating frequencies around it. |
| Low-cut / High-cut | Remove frequencies below or above a corner. |

Use **Q** to adjust width or resonance. Cut filters also provide a slope control. Controls that do not apply to the current shape are hidden.

Hover over a node and use the mouse wheel to adjust Q. On low-cut and high-cut nodes, the wheel adjusts slope. Double-click a gain-based node to return its gain to 0 dB. Right-click a node to delete that band; use its power button to switch it off while retaining its settings.

## Stereo, Mid, and Side

The **ST**, **M**, and **S** buttons select the curve you are editing:

- **ST:** process both channels.
- **M:** process the center component of a stereo signal.
- **S:** process the difference between the channels.

With a mono input, the interface shows **MONO** instead. Mid/Side processing requires a stereo signal.

## Dynamic EQ

Dynamics are available on bell, low-shelf, high-shelf, and tilt-shelf bands. Select a band and enable dynamics from its floating controls.

The band's gain sets the direction and maximum amount of the change. Negative gain applies a dynamic cut; positive gain applies a dynamic boost.

- **Threshold:** the detector level above which the band reacts.
- **At:** attack time, in milliseconds.
- **Rl:** release time, in milliseconds.
- **Sidechain:** use an external signal to trigger the band. Route that signal to the plugin's sidechain input in your DAW first.

The detector-listen control lets you hear the signal driving the selected band's dynamics. Hold to listen; release to return to the normal output.

## Band listening

Hold the band's headphones button to hear its frequency region. Drag sideways while holding to sweep the band, then release to return to the full signal. Band listening is unavailable on the tilt shelf.

## Analyzer and display

Open analyzer settings with the analyzer button at the bottom right. The analyzer shows the output spectrum.

- Larger FFT sizes give finer frequency resolution with a slower response.
- Smoothing reduces detail in the trace.
- Speed controls how quickly the display responds and falls.
- Peak hold retains a per-frequency peak line.

Use the range selector above the graph to change the vertical display range. This changes the view, not the band's gain. The theme selector is in the top bar.

## Presets and levels

Use the save button in the top bar to save a preset. Click the preset name to load a `.rookeq` file. Your DAW also saves the plugin's settings with the session.

The input and output trims sit beside their meters. Adjust output level when comparing processed and bypassed sound. Click a meter to clear its clip indicator.

## Feedback

See [Support](../SUPPORT.md) for bug-report details and the current development status.
