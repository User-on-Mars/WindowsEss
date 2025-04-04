# WindowsEss

✅ Batch Script: install-dev-tools.bat

@echo off
echo ===== Starting Dev Setup with winget =====

:: Update winget
echo Updating winget...
winget upgrade --all --silent

:: 1. VS Code
echo Installing VS Code...
winget install --id Microsoft.VisualStudioCode -e --silent

:: 2. WSL (you need to manually select SUSE later via Microsoft Store)
echo Installing WSL (requires reboot to finalize)...
wsl --install

:: 3. Python
echo Installing Python...
winget install --id Python.Python.3 -e --silent

:: 4. Selenium (install via pip after Python)
echo Installing Selenium (via pip)...
pip install selenium

:: 5. Java JDK 17
echo Installing Java JDK 17...
winget install --id Oracle.JDK.17 -e --silent

:: 6. Visual Studio Community Edition
echo Installing Visual Studio...
winget install --id Microsoft.VisualStudio.2022.Community -e

:: 7. Node.js
echo Installing Node.js...
winget install --id OpenJS.NodeJS.LTS -e --silent

:: 8. Git
echo Installing Git...
winget install --id Git.Git -e --silent

:: 9. GitHub Desktop
echo Installing GitHub Desktop...
winget install --id GitHub.GitHubDesktop -e --silent

:: 10. KDE Connect
echo Installing KDE Connect...
winget install --id KDE.KDEConnect -e --silent

:: 11. Mullvad Browser
echo Installing Mullvad Browser...
winget install --id Mullvad.MullvadBrowser -e

:: 12. Firefox
echo Installing Mozilla Firefox...
winget install --id Mozilla.Firefox -e --silent

:: 13. Vivaldi
echo Installing Vivaldi Browser...
winget install --id VivaldiTechnologies.Vivaldi -e --silent

:: 14. EarTrumpet
echo Installing EarTrumpet...
winget install --id File-New-Project.EarTrumpet -e --silent

:: 15. FxSound
echo Installing FxSound Enhancer...
winget install --id FxSoundLLC.FxSound -e --silent

:: 16. Voicemeeter Banana
echo Installing Voicemeeter Banana...
winget install --id VB-Audio.VoicemeeterBanana -e

:: 17. Equalizer APO
echo Installing Equalizer APO...
winget install --id EqualizerAPO.EqualizerAPO -e

:: 18. Peace GUI (manual install needed, open page)
echo Opening Peace GUI download page...
start https://sourceforge.net/projects/peace-equalizer-apo-extension/

:: 19. PowerToys
echo Installing PowerToys...
winget install --id Microsoft.PowerToys -e --silent

:: 20. Everything
echo Installing Everything Search Tool...
winget install --id voidtools.Everything -e --silent

:: 21. Obsidian
echo Installing Obsidian...
winget install --id Obsidian.Obsidian -e --silent

:: 22. Docker Desktop
echo Installing Docker Desktop...
winget install --id Docker.DockerDesktop -e

:: 23. Postman
echo Installing Postman...
winget install --id Postman.Postman -e --silent

:: 24. JetBrains Toolbox
echo Installing JetBrains Toolbox...
winget install --id JetBrains.Toolbox -e --silent

:: 25. ShareX
echo Installing ShareX...
winget install --id ShareX.ShareX -e --silent

echo ===== Installation Complete! Some apps may require reboot. =====
pause


✅ How to Use This

    Open Notepad

    Paste the script above.

    Save it as:

install-dev-tools.bat

Right-click the .bat file → Run as Administrator

Wait while your system becomes awesome 🚀
