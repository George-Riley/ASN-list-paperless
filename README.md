# **Paperless-NGX ASN Index Generator**

A streamlined Bash script designed specifically for the **Unraid User Scripts plugin**. It communicates with your Paperless-NGX API to generate a professional PDF index and a CSV backup of all documents containing an Archive Serial Number (ASN).

## **🚀 Compatibility**
* **OS:** Unraid v7.2.3 (Tested)
* **Dependencies:** `jq` (Standard on Unraid) and `Docker` (creates then removes a `wkhtmltopdf` container)

## **🛠️ Setup**
1. Open your **Unraid WebGUI**.
2. Navigate to **Settings** > **User Scripts**.
3. Click **Add New Script** and name it what you want.
4. Click the gear icon and select **Edit Script**.
5. Paste the script content and update these **bolded variables**:
    * **`PAPERLESS_URL`**: The full URL to your instance (e.g., `https://paperless.local`).
    * **`API_TOKEN`**: Your unique Paperless API token.
    * **`OUTPUT_DIR`**: The Unraid path where files should be saved (e.g., `/mnt/user/documents/`).
6. Set the **Schedule** to your preference.

## **📦 Output**
* **`Paperless_ASN_Index.pdf`**: A clean, printable table for physical filing reference.
* **`paperless_index.csv`**: A raw data export for spreadsheet use.

## **🗺️ Roadmap**
* [ ] **Email Updates**: Implement weekly email notifications that trigger only if the PDF content has changed (new documents added).
