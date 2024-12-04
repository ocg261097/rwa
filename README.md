# RWA - Restore WhatsApp (Magisk Module)

RWA is a Magisk Module designed to simplify the restoration of WhatsApp Personal or WhatsApp Business data from `.tar.gz` backup files. With this module, you can quickly restore important files and settings, making the process seamless for rooted devices.

## Features
- Restore WhatsApp Personal (`com.whatsapp`) or WhatsApp Business (`com.whatsapp.w4b`) backups.
- Automatically detects and processes the latest `.tar.gz` backup file.
- Restores:
  - `keystore.xml`
  - Shared preferences (`com.whatsapp_preferences_light.xml`)
  - Files in the `/files` directory.
- Copies the registered phone number to the clipboard.
- Logs restoration progress for easy debugging.

## Requirements
- Root access via [Magisk](https://magisk.me/).
- A device running Android.
- Backup files stored in one of the following directories:
  - `/sdcard/OCG/restore/com.whatsapp/` (for WhatsApp Personal).
  - `/sdcard/OCG/restore/com.whatsapp.w4b/` (for WhatsApp Business).

## Installation
1. Download and install [Magisk](https://github.com/topjohnwu/Magisk).
2. Download rwa module.
3. Flash the `rwa.zip` file in Magisk Manager:
4. Open Magisk Manager.
5. Go to Modules > Install from Storage.
6. Select the `rwa.zip` file and reboot.

## Usage
1. Open a terminal emulator (e.g., Termux) on your device.
2. Switch to superuser mode: su
3. Run the `rwa` command followed by the desired mode:
   - `wp`: Restore WhatsApp Personal.
   - `wb`: Restore WhatsApp Business.

### Example Command
$ `su -c rwa wp`


Restoring WhatsApp Personal Total tar.gz: 1 Nama File: backup_2023.tar.gz Nomor disalin: 6281234567890

## Troubleshooting
- Ensure backup files are in the correct directory:
  - `/sdcard/OCG/restore/com.whatsapp/`
  - `/sdcard/OCG/restore/com.whatsapp.w4b/`
- Verify required commands (`tar`, `am`, `pm`) are available on your device.
- Check logs for error messages.

## Contributing
Contributions, suggestions, and bug reports are welcome! Feel free to submit an issue or pull request.

## License
This project is licensed under the [MIT License](LICENSE).

---

**Powered by OCG**  
[GitHub Repository](https://github.com/ocg261097/rwa/)


