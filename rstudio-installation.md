# R & RStudio Setup
## IMBB Data Analysis Course — Week 2

Please complete these steps **before Week 2 begins**. This guide sets up a standalone R environment using RStudio Desktop.

Choose your operating system and follow the instructions.

---

## Windows

### 1. Install R

1. Go to [https://cran.r-project.org/bin/windows/base/](https://cran.r-project.org/bin/windows/base/)
2. Click **Download R x.x.x for Windows**
3. Run the downloaded `.exe` file and follow the setup wizard — default settings are fine

Verify by opening **Command Prompt** (search "cmd" in the Start menu) and typing:

```
R --version
```

If it prints version information, R is installed correctly.

### 2. Install RStudio Desktop

1. Go to [https://posit.co/download/rstudio-desktop/](https://posit.co/download/rstudio-desktop/)
2. As you have already installed R, go to **2: Install RStudio**
3. The site will detect Windows automatically — select your OS and download and run the `.exe` installer
4. Follow the setup wizard with default settings
5. Launch RStudio from the Start menu

### 3. Verify installation

Open RStudio. In the **Console** pane (bottom-left), paste the following and press Enter:

```r
print("All good.")
```

If it prints "All good." — the environment is ready.

### Windows troubleshooting

**R not found after installation**
Close and reopen Command Prompt. If it still says "command not found", try restarting your computer.

---

## macOS

### 1. Install R

Open **Terminal** (Applications → Utilities → Terminal, or press `Cmd+Space` and type "Terminal").

Go to [https://cran.r-project.org/bin/macosx/](https://cran.r-project.org/bin/macosx/) and download the appropriate installer:

- **Apple Silicon (M1/M2/M3/M4):** `R-x.x.x-arm64.pkg`
- **Intel Mac:** `R-x.x.x-x86_64.pkg`

Not sure which Mac you have? Click the Apple menu → About This Mac. If it says "Apple M1" or similar, it's Apple Silicon. If it says "Intel", it's Intel.

Open the `.pkg` file and follow the installation steps.

Verify in Terminal:

```bash
R --version
```

If it prints version information, R is installed correctly.

### 2. Install RStudio Desktop

1. Go to [https://posit.co/download/rstudio-desktop/](https://posit.co/download/rstudio-desktop/)
2. Download the macOS `.dmg` file
3. Open the `.dmg` and drag **RStudio** to your Applications folder
4. Launch RStudio from Applications or Spotlight (`Cmd+Space`, type "RStudio")

> **Note:** On first launch, macOS may warn about an unidentified developer. If it does so, go to **System Settings → Privacy & Security** and click **Open Anyway**.

### 3. Verify installation

Open RStudio. In the **Console** pane (bottom-left), paste the following and press Enter:

```r
print("All good.")
```

If it prints "All good." — the environment is ready.


### macOS troubleshooting

**"xcrun: error: invalid active developer path"**
macOS is asking you to install command-line tools. Run `xcode-select --install`, follow the prompt, then try again.

**RStudio doesn't detect R**
Go to **Tools → Global Options → General** and manually set the R version path (usually `/usr/local/bin/R` for Intel or `/opt/homebrew/bin/R` for Apple Silicon).

---

## Still stuck?

Email the Week 2 instructors before Week 2 starts, so that they can help with any remaining setup issues.
