# DCTL Tools

Creative color tools by Elliott Powell for DaVinci Resolve Studio.

## Installation

Copy the `.dctle` files from [Creative Tools](creative-tools/) into your Resolve LUT folder:

**macOS:** `/Library/Application Support/Blackmagic Design/DaVinci Resolve/LUT`

**Windows:** `C:\ProgramData\Blackmagic Design\DaVinci Resolve\Support\LUT`

Restart Resolve, add the DCTL effect to a node, and select the desired tool.

---

## HellwigHueMesh

Adjust hue, saturation, and brightness of six color regions using a tetrahedral mesh in the Hellwig color appearance model.

---

## SaturationDensity

Shape saturation and density with a choice of RGB and perceptual models.

### Saturation models

- **Additive:** Simple log-based additive saturation.
- **Log HSV:** Log-based HSV saturation. Subtractive like appearance.
- **Luminance Preserving:** Adjusts saturation in linear light while preserving luminance.
- **Perceptual (Hellwig HK):** Adjusts colorfulness using the Hellwig appearance model with the Helmholtz–Kohlrausch extension, aiming to preserve model brightness and hue.

### Density models

Positive Density darkens more colorful pixels; negative Density brightens them. Saturation is applied before density.

- **RGB Minimum-Based:** Darkens colors based on the difference between their strongest and weakest RGB channels. Affects different hues more evenly than Average-Based.
- **RGB Average-Based:** Darkens colors based on the difference between their strongest channel and the average of all three channels. Gives different emphasis to different hues.
- **Perceptual (Hellwig HK):** Darkens colors based on their colorfulness in the Hellwig appearance model, while preserving model saturation and hue. Affects all hues evenly.

---

## License and notices

Available for personal and commercial grading under the [Interim Use License](LICENSE.md). These encrypted tools are not open source. Redistribution and code reuse in distributed products require permission; finished images and videos do not.

See [third-party notices](THIRD_PARTY_NOTICES.md). The Colour BSD-3-Clause notice accompanies the encrypted tools.
