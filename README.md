## Master Healer Kale Trainer

A small companion app for **Master Healer Kale** that lets you see and change your **Gold, Skill Points, and Ruby** while the game is running.

Created by **Arzharoth**. This is an unofficial project, not affiliated with or endorsed by the game's developer.

### Download

**[Download v0.1.0 for Mac — Apple Silicon](https://github.com/yveschiong/master-healer-kale-trainer-releases/releases/download/v0.1.0/Master-Healer-Kale-Trainer-0.1.0-macOS-arm64-experimental.zip)**

[Release notes and all downloads](https://github.com/yveschiong/master-healer-kale-trainer-releases/releases)

> **Experimental release:** back up your game save before using it. Changes apply immediately and may be saved by the game. There is no undo.

### What can it do?

- **See your resources live:** Gold, Skill Points, and Ruby refresh automatically after you unlock the trainer.
- **Set a new amount:** enter the full amount you want, then click **Set** next to that resource.
- **Read large numbers more easily:** amounts use comma separators rather than abbreviated suffixes.
- **Run as a normal Mac app:** everything needed by the trainer is bundled. No coding tools, Cheat Engine, or separate helper installation is required.

### What you'll need

| Requirement | Details |
| --- | --- |
| Mac | Apple Silicon, such as an M1, M2, M3, or M4 Mac. Intel Macs are not supported. |
| macOS | Built for macOS 13 or later; locally tested only on the developer's macOS 26 Mac. |
| Game | Master Healer Kale installed and running under your Mac user account. Run only one copy at a time. |
| Permission | macOS administrator approval when you click **Unlock trainer**. |

**There is no Windows build.** Compatibility across game versions has not been established, and game updates may break the trainer.

Not sure which Mac you have? Open **Apple menu → About This Mac** and check the **Chip** or **Processor** entry.

### Install and get started

1. **Back up your game save.** Keep a copy you can restore if something goes wrong.
2. **Download the app ZIP** using the link above. If you're on the release page, choose `Master-Healer-Kale-Trainer-0.1.0-macOS-arm64-experimental.zip` under **Assets**.
3. **Open the ZIP**, then move the complete `Master Healer Kale Trainer.app` to **Applications**. Do not remove files from inside the app.
4. **Launch the game** and load your save, then open the trainer.
5. **Click Unlock trainer** and review the macOS administrator prompt before approving it.
6. **Compare the displayed resources with the game.** If they do not match, stop—do not click **Set**.
7. **Try a small change first.** Enter your desired total for one resource, click **Set**, and check the result in the game.

**Set replaces the amount; it does not add to it.** For example, entering `1,000` sets that resource to 1,000, rather than adding 1,000.

Gold accepts decimal amounts. Skill Points and Ruby require whole numbers. Use full numbers, not suffixes such as `M` or `Q`; commas are accepted. All amounts must be nonnegative, and the maximum editable amount is **9,007,199,254,740,991**. Very large amounts may lose some precision.

Closing the trainer or restarting the game ends the session. Click **Unlock trainer** again when you're ready to reconnect.

### If macOS blocks the app

This experimental build is **not Developer ID signed or notarized by Apple**, so macOS may warn about it or prevent it from opening.

Only if you trust this download:

1. Try opening the app from **Applications**.
2. Open **System Settings → Privacy & Security**.
3. Look for the message about the trainer and choose **Open Anyway**, if available. Review the next prompt before proceeding.

**Do not disable Gatekeeper or System Integrity Protection (SIP).** A work or school Mac may have policies that prevent the app from running. This release does not bypass those policies.

The app uses ad-hoc signing, which does not establish the publisher's identity. A warning-free launch on the developer's Mac does not mean downloaded copies will open without warnings.

### Why does it ask for administrator permission?

The trainer needs permission to read and change resources in the running game. Clicking **Unlock trainer** starts a bundled helper with administrator privileges for that session; the trainer window itself stays unprivileged.

Your password is entered in the **macOS prompt**, not collected or stored by the trainer. No permanent background service is installed. You may be asked to approve again after restarting the trainer or game.

### Troubleshooting

| What you see | What to do |
| --- | --- |
| Game not detected | Start the game under the same Mac account, keep only one copy running, and click **Refresh** in the trainer. |
| Unlock fails or access is denied | Check that the game is still running and that you approved the macOS prompt. Permission approval does not guarantee macOS will allow access; do not weaken system security settings. |
| Resources look wrong | Stop using the trainer. A game update may have changed where resources are stored, and plausible-looking numbers are not proof of compatibility. |
| An error after clicking Set | Check the game before trying again: the change may already have applied. The trainer does not automatically retry or undo writes. |
| The trainer locks again | Sessions can end after inactivity, errors, a game restart, or eight hours. Check the game, then unlock again. |

For help, [open an issue](https://github.com/yveschiong/master-healer-kale-trainer-releases/issues) with your trainer version, game version, macOS version, Mac chip, and the exact error message. If available, include relevant details from **Advanced**, but leave out passwords and personal information.

### Optional: check your download

The release includes a `.sha256` file to check whether the ZIP matches the published checksum. Download both files into the same folder, then run this in Terminal from that folder:

```sh
shasum -a 256 -c Master-Healer-Kale-Trainer-0.1.0-macOS-arm64-experimental.zip.sha256
```

The result should end with **OK**. If it does not, do not open the app; download it again from the release page. A checksum checks file integrity, not whether the publisher or app is trustworthy.

### About this repository

This repository hosts **downloads and release information only**. The game is not included, and the trainer's application source is not published here.

GitHub automatically adds **Source code (zip)** and **Source code (tar.gz)** to releases. Those are repository snapshots, **not the trainer app**. Use the named app ZIP instead.
