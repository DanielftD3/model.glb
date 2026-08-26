Austroraptor - original source texture export

This package intentionally contains the original PNG pixels exported from the game.
No recoloring, normalization, dithering, darkening, threshold correction, or WebP conversion was applied.

Files:
- pattern_1.png: exact copy of T_Austroraptor_Adult_Pattern_1.png
- pattern_2.png: exact copy of T_Austroraptor_Adult_Pattern_2.png
- pattern_3.png: exact copy of T_Austroraptor_Adult_Pattern_3.png
- pattern_4_heron.png: exact copy of T_Austroraptor_Adult_Pattern_Heron_M.png
- normal.png: exact copy of T_Austroraptor_Adult_N.png
- mask_tmc.png: exact copy of T_Austroraptor_M.png
- pattern_blend_source_colors.csv: separate lookup table for special source RGB values situated in the Flank-to-Markings color corridor. This table does not modify the textures.
- alpha_channel_report.csv: alpha-channel verification for every supplied texture.
- SHA256SUMS.txt: hashes proving the supplied image files match the extracted sources.

Alpha warning:
All provided game-export PNG files are RGBA, but their exported alpha channel is uniformly 255 (fully opaque). Therefore, the available sources do not contain a useful cutout/opacity mask. A real removal mask must be exported from another game asset or authored separately. The original alpha channel is preserved exactly; no alpha was invented.

Rendering:
Keep the source RGB values unchanged. Any darkening or material response should occur at render time, as in the game.
