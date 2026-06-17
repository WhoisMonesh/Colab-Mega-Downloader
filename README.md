# Mega Downloader

Download files from Mega.nz links directly to Google Drive.

[![Open In Colab](https://colab.research.google.com/assets/github/WhoisMonesh/Colab-Mega-Downloader/blob/main/Colab-Mega-Downloader.ipynb)]

---

## Features
| Feature | Description |
|---|---|
| **Sync-safe** | Downloads to local temp, moves to Drive after |
| **Progress Bar** | Real-time HTML progress |
| **Keep-Alive** | Prevents Colab timeout |
| **Auto-Zip** | Zips multiple files with progress + download link |

## How to Use
1. Mount Google Drive
2. Install dependencies
3. Configure variables
4. Run download

### Configuration
| Variable | Default | Description |
|---|---|---|
| `SAVE_PATH` | `/content/downloads/.../` | Local temp dir |
| `DRIVE_PATH` | `/content/drive/My Drive/.../` | Final Drive destination |
| `MEGA_LINK` | `""` | Mega.nz file/folder link |
| `MEGA_EMAIL` | `""` | Mega account email (optional) |
| `MEGA_PASSWORD` | `""` | Mega account password |
| `KEEP_ALIVE` | `True` | Prevent Colab timeout |

### Features
- Download from Mega.nz links
- Optional account login for higher transfer limits
- Folder download support

---

## Technical Details
- Downloads to `/content/downloads/` first, then moves to Drive
- Uses IPython.display HTML for live progress updates
- JavaScript keep-alive prevents session timeout

## Disclaimer
For legal use only.

## License
MIT
