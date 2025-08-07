Step-by-Step Instructions (Using Git Bash on Windows)

**Pin** `about:debugging` on Firefox
```
about:debuggin
```

🧩 Step 1: Create a Clean ZIP Package

    In your Git Bash terminal, navigate to your extension directory:

```
cd /f/github/Share-2-Telegram-main
```

Create a ZIP file excluding the .git folder and unnecessary files like README.md or LICENSE.

You can do it with this command:
Powershell
``
```powershell
cd F:\github\Share-2-Telegram-main

```

```
zip -r share2telegram.zip background.js icons lib manifest.json options.html options.js
```

If you want to include the LICENSE, feel free to add it.

Optional: Rename the zip to .xpi (Firefox add-on format):

```
mv share2telegram.zip share2telegram.xpi
```

🦊 Step 2: Load the Extension in Firefox

There are 2 options:
Option A: Temporary Load (easier for testing)

    Open Firefox.

    Go to: about:debugging

    Click "This Firefox".

    Click "Load Temporary Add-on..."

    Browse to your folder and select the manifest.json file.

    Your extension will be installed temporarily until Firefox restarts.