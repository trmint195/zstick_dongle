# ZStick dongle

## 🔐 Setup 2.4G AES Encryption Key

To generate a random 128-bit AES Key for secure wireless communication and compile your firmware:

1. Go to the **Actions** tab in your GitHub repository.
2. In the left sidebar, select **Generate AES Key and Build**.
3. Click the **Run workflow** dropdown menu on the right.
4. Select your branch (e.g., `main`) and click **Run workflow**.

> **Note:** This action automatically scans all `.conf` files in the `config/` directory for `CONFIG_ZMK_2G4_AES_KEY`, updates them with a matching random 32-character hexadecimal key, commits the changes to your repository, and triggers the ZMK firmware build process immediately. Subsequent standard builds will reuse this generated key.
