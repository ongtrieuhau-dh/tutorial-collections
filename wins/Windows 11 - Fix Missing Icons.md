# Hướng dẫn sửa lỗi mất icon trên Windows 11

To fix the missing icons on Windows 11, you can try the following steps:

1. **Restart Windows Explorer:**
   - Press `Ctrl + Shift + Esc` to open Task Manager.
   - Scroll down to find "Windows Explorer."
   - Right-click on "Windows Explorer" and select "Restart."

2. **Rebuild the Icon Cache:**
   - Press `Win + R` to open the Run dialog.
   - Type `cmd` and press `Ctrl + Shift + Enter` to open Command Prompt as an administrator.
   - In the Command Prompt, enter the following commands one by one:

     ```shell
     taskkill /f /im explorer.exe
     cd /d %userprofile%\AppData\Local
     del IconCache.db /a
     start explorer.exe
     ```

3. **Check for Updates:**
   - Go to `Settings` > `Windows Update`.
   - Click on `Check for updates` and install any available updates.

4. **Reset Icon Cache Using File Explorer Options:**
   - Open `File Explorer`.
   - Go to `View` > `Options` > `Change folder and search options`.
   - In the Folder Options window, go to the `View` tab.
   - Check the box "Always show icons, never thumbnails."
   - Click `Apply` and then `OK`.
   - Restart your computer and then uncheck the box again.

5. **Restore Default Icons:**
   - Right-click on the desktop and select `Personalize`.
   - Go to `Themes` and select `Desktop icon settings`.
   - Click on `Restore Default` and then click `Apply` and `OK`.

Try these steps, and if the issue persists, let me know for further assistance.
