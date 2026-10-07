You are producing desktop wallpapers for an Omarchy theme. Read prompts/WALLPAPER-BRIEF.md first and follow it exactly.

Task:
1. For each of the 4 layouts in the brief, generate the image three times with your built-in image generation tool: once composed for 16:9, once for 21:9 ultrawide, once for 16:10. That is 12 generations. Request the largest landscape size the tool offers each time. For the 21:9 and 16:10 versions, pass the finished 16:9 image as the reference so the three read as the same scene recomposed, not three different pictures.
2. Look at every result yourself. If one breaks a rule in the brief (text, a recognisable franchise character, too bright, subject in the wrong place, flat or blobby), regenerate it with a corrected prompt. Up to 3 attempts per image.
3. Bring each accepted image to its exact final size from the brief's table with ImageMagick (`magick`): crop to the exact aspect ratio keeping the subject, then Lanczos resize. Do not stretch.
4. Save as JPEG quality 92 with these names:
   - backgrounds/01-heat-signature.jpg, 02-tri-laser.jpg, 03-cloak.jpg, 04-isotherm.jpg
   - backgrounds-ultrawide/ with the same four names
   - backgrounds-16x10/ with the same four names
5. Next to prompts/WALLPAPER-BRIEF.md, write prompts/<name>-<aspect>.prompt.txt for each final image holding the exact prompt that produced it.
6. Verify with `magick identify` that all 12 files exist at the exact sizes, and print that listing as your final message along with one line per image on anything you were not happy with.

Do not modify colors.toml, btop.theme, icons.theme or backgrounds/00-procedural-placeholder.png. Do not create any other files in the repo root. Do not run git commands.
