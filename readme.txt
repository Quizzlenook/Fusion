## Fusion Overlay for Hypixel Bedwars

### Download
Click one of the direct download buttons above, or [click here][latest-release-link-fusion] to view the latest release of Fusion. Your browser might display a warning about the file being potentially harmful, but rest assured this is a standard warning. Please refer to our [safety](#safety) section below for more details.

**NOTE for Mac users:** The first time you launch Fusion on a Mac, you might have to use the shift+right click combination on the application and select "Run".

### Support and Feedback
For assistance with the Fusion setup or if you have any feedback to share, join our [discord server][discord-invite-link-fusion]. We also welcome issues or pull requests on GitHub.

### Description
Fusion is an innovative, open-source overlay tailored for Hypixel Bedwars (independent project). Fusion automatically recognizes players in your lobby and displays their stats upon entering `/who`. Integration with the [Antisniper API](https://antisniper.net) (unaffiliated) is available for additional features.

### Features
- Seamless party and lobby detection.
- Personalized stats table.
- Top-tier players are highlighted for easy identification.
- Quick and lightweight performance.
- Integration with Discord to display session stats.
- Capability to identify disguised players with the Antisniper API.
- Predictive win streaks using the Antisniper API.

### Pro Tips
- Use autowho to avoid typing `/who` every time.
- For Windows users, use the "Fullscreen" button to position Fusion over fullscreen Minecraft.
- For advanced features like identifying disguised players, add your Antisniper API key following the steps in the settings.

### Known Issues

**Show on tab glitch when shift is pressed:**  
This is due to key changes when the shift is held (e.g., Shift+1 becomes !). We recommend using letter keys or special keys for this function.

**Overlay doesn't display on Mac when tab is pressed:**  
This is a known library issue and may not be addressed soon. However, the overlay will still automatically launch when a game begins.

**Overlay invisibility on Linux:**  
Switching workspaces might resolve this. If not, refer to the secret setting `disable_overrideredirect` in our [previous PR](https://github.com/Ukrane211/fusion/pull/1).

**Overlay focusing issue on Linux:**  
The `hide_with_alpha` secret setting might help. Details can be found in [this PR](https://github.com/Ukrane211/fusion/pull/1).

### Safety
Being open-source, Fusion's code is available for scrutiny, ensuring user safety. The binaries are generated via GitHub Actions from a fresh clone. Skeptical users can run the project from the source code after reviewing it.

### Running Fusion from Source
Ensure you have Python `>=3.11`.

**Steps:**

1. **Clone the repository:**
    ```bash
    git clone https://github.com/Ukrane211/fusion
    ```

2. **Setup a virtual environment (optional):**  
    Follow the steps similar to the ones mentioned in the Prism readme.

3. **Install dependencies:**
    ```bash
    pip3 install -e . -r requirements/<os>.txt
    ```

4. **Run Fusion:**
    ```bash
    python3 fusion_overlay.py
    ```

For command line arguments, use:
```bash
python3 fusion_overlay.py --help
```

### Developer Information
Username: `Ukrane`  

[latest-release-link-fusion]: https://github.com/Ukrane211/fusion/releases/latest
[discord-invite-link-fusion]: https://discord.gg/k4FGUnEHYg