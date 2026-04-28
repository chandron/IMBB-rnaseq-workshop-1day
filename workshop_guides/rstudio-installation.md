# R & RStudio Setup
## IMBB Data Analysis Course — Week 2

Please complete these steps **before Week 2 begins**. This guide sets up a standalone R environment using RStudio Desktop.

Choose your operating system and follow the instructions.

---

## Windows

### 1. Install R

1. Go to [https://cran.r-project.org/bin/windows/base/](https://cran.r-project.org/bin/windows/base/)
2. Click **Download R x.x.x for Windows**
3. Run the downloaded `.exe` file and follow the setup wizard — default settings are fine (an R desktop icon is not really necessary)

Once the installation finishes, continue to Step 2. You will verify R is working from inside RStudio.

### 2. Install RStudio Desktop

1. Go to [https://posit.co/download/rstudio-desktop/](https://posit.co/download/rstudio-desktop/)
2. As you have already installed R, go to **2: Install RStudio**
3. The site will detect Windows automatically — run the `.exe` installer
4. Follow the setup wizard with default settings
5. Launch RStudio from the Start menu

### 3. Verify installation

Open RStudio. In the **Console** pane, paste the following and press Enter:

```r
print("All good.")
```

If it prints "All good." — the environment is ready.

For this course you will also need to install rmarkdown package.  
All you need to do is run: 
```r
install.packages("rmarkdown")
```

Done!

---

## macOS

### 1. Install R

Open **Terminal** (Applications → Utilities → Terminal, or press `Cmd+Space` and type "Terminal").

Go to [https://cran.r-project.org/bin/macosx/](https://cran.r-project.org/bin/macosx/) and download the appropriate installer:

- **Apple Silicon (M1/M2/M3/M4):** `R-x.x.x-arm64.pkg`
- **Intel Mac:** `R-x.x.x-x86_64.pkg`

  Not sure which Mac you have? Click the Apple menu → **About This Mac**. If it says "Apple M1" or similar, it's Apple Silicon. If it says "Intel", it's Intel.

Open the `.pkg` file and follow the installation steps. 

Verify in Terminal:

```bash
R --version
```

If it prints version information, R is installed correctly.

### 2. Install RStudio Desktop

1. Go to [https://posit.co/download/rstudio-desktop/](https://posit.co/download/rstudio-desktop/)
2. As you have already installed R, go to **2: Install RStudio**
3. The site will detect macOS automatically — select your OS and download and run the `.dmg` installer

   Not sure which macOS version you have? Run this in the Terminal:

  ```bash
  sw_vers -productVersion
  ```

  If it prints `14.x.x` or higher, select **macOS 14+**. If it prints `13.x.x` or lower, select **macOS 10.12 - 13**.
  
4. Launch RStudio from Applications or Spotlight (`Cmd+Space`, type "RStudio")

> **Note:** On first launch, macOS may warn about an unidentified developer. If it does so, go to **System Settings → Privacy & Security** and click **Open Anyway**.

### 3. Verify installation

Open RStudio. In the **Console** pane, paste the following and press Enter:

```r
print("All good.")
```

If it prints "All good." — the environment is ready.


For this course you will also need to install rmarkdown package.  
All you need to do is run: 
```r
install.packages("rmarkdown")
```

Done!

---

## Linux

### 1. Install R

Open a **Terminal** and run the following commands. These instructions are for Debian/Ubuntu-based distributions (e.g., Ubuntu, Linux Mint). For other distributions, see [https://cran.r-project.org/bin/linux/](https://cran.r-project.org/bin/linux/).

```bash
sudo apt update
sudo apt install -y r-base
```

Verify:

```bash
R --version
```

If it prints version information, R is installed correctly.

### 2. Install RStudio Desktop

1. Go to [https://posit.co/download/rstudio-desktop/](https://posit.co/download/rstudio-desktop/)
2. As you have already installed R, go to **2: Install RStudio**
3. Select your Linux distribution and download the appropriate `.deb` package

   Not sure which distribution you have? Run this in the Terminal:

   ```bash
   cat /etc/os-release
   ```

   Look for the `NAME` and `VERSION_ID` lines — for example, `Ubuntu 22.04` or `Ubuntu 24.04`. Use this to select the matching option on the RStudio download page.

4. Install it from the Terminal (replace the filename with the one you downloaded):

```bash
cd ~/Downloads
sudo dpkg -i rstudio-*.deb
sudo apt --fix-broken install
```

5. Launch RStudio by typing `rstudio` in the Terminal, or find it in your applications menu

### 3. Verify installation

Open RStudio. In the **Console** pane, paste the following and press Enter:

```r
print("All good.")
```

If it prints "All good." — the environment is ready.

For this course you will also need to install rmarkdown package.  
All you need to do is run: 
```r
install.packages("rmarkdown")
```

Done!

### Linux troubleshooting

**`dpkg` errors during installation**
Run `sudo apt --fix-broken install` after the `dpkg` command — this resolves most missing dependency errors.

**RStudio not found after installation**
Try launching from the Terminal with `rstudio`. If the command is not found, reboot and try again.

**Permission errors when installing packages in R**
R may be trying to install to a system directory. When prompted, type `yes` to install to a personal library instead (usually `~/R/`).

---

## 📧 Contact & Support

If you are stuck on any setup issues, email the Week 2 instructors before Week 2 starts, we are happy to help!

| Name | Email |
|---|---|
| Christos Andronis | ch.andronis@imbb.forth.gr |
| Electra Tsaglioti | electra_tsaglioti@imbb.forth.gr |
