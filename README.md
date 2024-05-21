### Fork From [ctn](https://github.com/ctn123)
Using Frame4 Instead Of PS4Debug

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/X8X741UC0)

If you like my builds, please donate to help fund the development of PS4 Cheater and ps4debug.

# PS4_Cheater & ps4debug

PS4 Cheater is a homebrew application to find game cheat codes. It is based on [ps4debug](https://github.com/jogolden/ps4debug).

### Supported Firmware: 5.04, 9.00, 11.00.

### Latest version: 1.5.4.7
  - Please find all new releases (with Changelog) here: https://github.com/ctn123/PS4_Cheater/releases.
  - Public version of Unified ps4debug.bin and libdebug.dll are also on the releases page.
  - This version has ps4debug that survives rest mode (Under testing, please report any bugs)

Note: Closed source from 1.5.3 onwards.

### Notable new features (v1.5.0 onwards):
  - Ported from jkpatch to ps4debug (new supports for 7.02, 7.5X and 9.00)
  - Performance that significantly exceeds the old PS4 Cheater (jkpatch) versions 1.4.8 and below.
  - Console scanner which does the scanning on the ps4 console.
  - Firmware agnostic ps4debug payload
    - One payload for all firmware (5.0X, 6.72, 7.02, 7.5X, 9.00)
    - No longer required to select firmware from the drop down.
  - Multi-threaded scanning
  - Auto-pause function
  - ps4debug with Rest Mode support (survives through rest mode)

### Performance tips:
  - Console scanner
    - Fast but not always faster than the non-console scanner.
  - auto-pause enables scans to happen faster, for games that support it.
    - Some games will crash when auto-pause on, so experiement with it.
  - Use Unknown Initial Low Value to filter out useless high values to speed up scans.
    - Use this instead of the standard Unknown Initial Value scan.
  - You can enable console scanner for the first scan, then disable for the next scan etc.
    - Can mix and match
  - If you can't find the value you are looking for:
    - Try unchecking Alignment
    - Try unchecking Filter

### Troubleshooting:
  - Trouble connecting?
    - Try port 9020 / 9021 / 9090, depends on your bin loader.
    - Send the payload with PS4 Cheater with the included embedded payload.
  - Auto-pause causing the game to drop back to xmb or experience a crash/kp?
    - Disable auto-pause - Game is not compatible with this feature
  - Pause/Resume buttons causing the game to drop back to xmb or experience a crash/kp?
    - Don't use pause/resume - Game is not compatible with this feature
  - Can't find the value you are looking for?
    - Uncheck alignment and try again
    - Uncheck filter, refresh and try again
  - Found a value but can't added the address with the error "Address is out of range"
    - The section probably got deallocated/removed.
  - PS4 Cheater doesn't connect after waking from rest mode
    - Restart PS4 Cheater and hit refresh
    - Wait for rev1 :)
  - ps4debug doesn't survive through Rest mode?
    - Try with GoldHen 2.0b2, Hen 2.1.3b, Hen 2.1.4
  - PS4 sometimes doesn't wake after a few attempts
    - Known issue with GoldHen 1.1, wait for a fix.

### Recommended setup and usage
  1. Start PS4
  2. Wait 30s.
  3. Hen
  4. ChendoChap's binloader
  5. Start PS4 Cheater
  6. Send payload
  7. Refresh
  8. Find your cheats.

### Upcoming release: (So you can see what I am working on)
  - Increase reliability of ps4debug.
  - Increase performance of ps4debug

## Acknowledgements & Thanks!

- Countless contributors to `jkpatch`, `ps4-ksdk`, `ps4-payload-sdk`, `ps4debug` and `PS4_Cheater`.
- hejran7 for spending countless hours helping me test.
- [DeathRGH](https://github.com/DeathRGH) for the speedfix tweak for ps4debug.
- [Al-Azif](https://github.com/Al-Azif) for his [ps4-exploit-host](https://github.com/Al-Azif/ps4-exploit-host) - Very useful for local testing.

---
Discord chat site: https://discord.gg/PwBwUKf.
Please join us!
