# f-r-i-d-a-y-assets

Public asset hosting for the **F.R.I.D.A.Y.** X content system.

## Purpose

This repository stores images and videos generated for posts. Files are served via GitHub raw URLs so they can be used directly with Buffer's `create_post` API (which requires public HTTPS media URLs).

## Usage

Assets are uploaded via the script in the main F.R.I.D.A.Y. project:

```bash
./scripts/upload-asset.sh "temp/media/your-file.jpg" visuals
./scripts/upload-asset.sh "temp/media/your-video.mp4" visuals
```

The script returns a stable raw URL like:
`https://raw.githubusercontent.com/Oxyd22/f-r-i-d-a-y-assets/main/visuals/your-file.jpg`

## Folder Structure

- `visuals/` — General post visuals (images + videos)
- `posts/YYYY-MM-DD/` — Optional date-organized visuals

## Notes

- This repo must stay **public** (raw GitHub URLs require no authentication).
- Do not commit source files or large binaries outside of intentional post assets.
- Part of the F.R.I.D.A.Y. minimal high-signal X content system.
