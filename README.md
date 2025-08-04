# CompatibilityAPI ✨

A library created to allow modern applications to run on Windows 8.1.

## Usage

For the initial setup, run `setup.bat`. Once the installation is complete:

```bash
coaload.exe <path\to\application\example.exe> or -cfg example.txt
```

can be used in this way.
After running the setup, a desktop shortcut for `user.bat` will also be available.

## Application Compatibility ✔

Support for Chromium-based applications is being worked on. If you test the test builds on Chromium and open an issue with any problems you encounter (if any), you’ll be making a major contribution to development.
As in the previous version, I haven’t created a list yet — I probably will. You can also report working programs via the issues section.
I haven’t seen major issues with other software. If there are programs that don’t work, please report them with the error code starting with “C” if available, or the Windows error code (such as “entry point not found”), or a screenshot of the error. As I said above, this helps greatly with development.

![Screenshot 2025-06-27 223546](https://github.com/user-attachments/assets/0f121b92-a8d0-4331-b657-085bbd4229d3)

## What do the message boxes starting with “C” mean?

They were added intentionally and are used in the code as `testbox(L"example")`. They help identify which API is causing issues. If I’ve written an API call incorrectly, I can better understand the error using the last message box code shown before the crash.
If such a message box appears at startup or during use, please take note of it. It helps diagnose problems like system freezes or crashes.
This feature is planned to be only in test versions, but I might bring it to the main release as well.
