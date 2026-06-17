# Mega Downloader

Download files and folders from Mega.nz links directly to Google Drive with chunk-level live progress.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/WhoisMonesh/Colab-Mega-Downloader/blob/main/Colab-Mega-Downloader.ipynb)

---

## Features
| Feature | Description |
|---|---|
| **File + Folder support** | Single files and nested folder trees |
| **Live Progress** | Chunk-level HTML progress per file |
| **Account login** | Optional login for higher transfer limits |
| **Sync-safe** | Downloads to local temp, moves to Drive after |
| **Keep-Alive** | Prevents Colab timeout |
| **Auto-Zip** | Zips multiple files with progress + download link |
| **Large File Safe** | >500 MB files get a Drive link instead of browser download |

## How to Use
1. Mount Google Drive
2. Install dependencies
3. Configure variables
4. Run download

### Configuration
| Variable | Default | Description |
|---|---|---|
| `SAVE_PATH` | `/content/downloads/MegaDownloader/` | Local temp dir |
| `DRIVE_PATH` | `/content/drive/My Drive/MegaDownloader/` | Final Drive destination |
| `MEGA_LINK` | `""` | Mega.nz file/folder link |
| `MEGA_EMAIL` | `""` | Mega account email (optional, for higher limits) |
| `MEGA_PASSWORD` | `""` | Mega account password |
| `KEEP_ALIVE` | `True` | Prevent Colab timeout |

---

## Disclaimer / Fair Use

This tool is provided for **educational and personal use only**. You are responsible for complying with:

| Policy | Notice |
|---|---|
| **Mega ToS** | Using this tool must comply with Mega's Terms of Service. |
| **Copyright Law** | Only download content you have the legal right to access. |
| **Local Laws** | Ensure compliance with applicable copyright laws in your jurisdiction. |

By using this software, you agree to use it **lawfully and responsibly**. The author assumes no liability for misuse.

---

## Technical Details
- Downloads to `/content/downloads/` first, then moves to Drive
- Uses IPython.display HTML for live chunk-level progress
- JavaScript keep-alive prevents session timeout
- Large files (>500 MB) skip browser download — use Drive link instead
- Folder nodes are handled recursively with subdirectory preservation

## License
MIT
