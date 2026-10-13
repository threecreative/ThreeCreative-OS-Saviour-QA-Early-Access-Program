# Saviour — QA Review Test Plan (Invite-only)

Instructions
- This document is for invited QA reviewers only.
- For each test case: mark Pass / Fail / Blocked, attach logs/screenshots, and create an issue when problems are found.

## 1) Boot & Install
  - [ ] VM: Boot the image in QEMU/VirtualBox (use README in main repo).
  - [ ] USB: Write image to USB with Rufus (Windows) or dd (Unix); verify boot.
  - [ ] Document any BIOS/UEFI settings required and exact steps taken.

## 2) Tile UI behavior
  - [ ] Mouse: Click and interact with each tile (clock, calculator, files, settings).
  - [ ] Keyboard: Navigate tiles with Tab/arrow keys; open/close apps.
  - [ ] App lifecycle: Launch app, use, close, relaunch.

## 3) Networking & Octell
  - [ ] Wi‑Fi: Connect to secured network (PSK) and record time-to-connect.
  - [ ] Octell: Load http and https pages; test TLS error handling and basic navigation.
  - [ ] Offline: Confirm graceful error messages when no network.

## 4) File manager
  - [ ] Read/write: Create/edit/save a text file, verify persistence after reboot.
  - [ ] File operations: create folder, rename, delete, move.
  - [ ] Permissions: Verify any file permission handling (if applicable).

## 5) Apps & Games
  - [ ] Launch each bundled app and game; verify controls and expected behavior.
  - [ ] Command prompt: run basic commands (dir/ls, type/cat a file).

## 6) Defender & Security
  - [ ] Run Defender scan on a test folder and verify results are reported.
  - [ ] Confirm scan performance and no false-critical failures for safe test files.

## 7) Stability and performance
  - [ ] 30-minute stability session with multiple apps opened.
  - [ ] Reboot test: cold boot and warm reboot; verify no corruption.
  - [ ] VM memory variations (512MB/1GB) — note performance differences.

## 8) Diagnostics & logs
  - [ ] Collect system logs per the bug template instructions.
  - [ ] Record exact reproduction steps for any failures and attach artifacts.

## Severity classification
- Blocker: crash or data corruption that prevents further tests
- Major: core feature broken (networking fails entirely)
- Minor: UX or feature misbehaves but testing can continue
- Trivial: typos, small visual issues

## Recordkeeping
- Use the issue templates. Include tester handle, date/time, platform details, and attachments.
