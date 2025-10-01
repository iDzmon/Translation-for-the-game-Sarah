# 🗂️ Translation Base Zone

Welcome to the **translation base zone**.
This folder contains the game’s **original and unmodified files**, which serve as the foundation for all community-made translations.

---

## 📌 Purpose

* Provide the **raw files** needed to create or update translations.
* Act as a **safety/backup zone** — if something breaks during translation, you can restore the original files from here.
* Serve as a starting point for translations into **any language**.

---

## 📦 What’s inside?

* **Original game files** (untranslated).
* Organized structure according to the game’s data.
* Ready to be copied and used in translation projects.

---

# 🛠️ How to Edit the Translation (v1)

This version uses a simple **CSV file** for translations.

---

## 📋 Step by Step

1. **Open the CSV file**

   * Locate the translation file: `localization.csv`.
   * Open it with your preferred editor (Excel, LibreOffice, Google Sheets, or even a text editor).

2. **Edit the content**

   * Modify the text entries with your translations.
   * Save the file when finished.

3. **Place the modified file in the game folder**

   * Copy your updated CSV file to:

   ```
   /SarahsHouse_Data/StreamingAssets/Translation/localization.csv
   ```

4. **Run the game**

   * Start the game normally and your translation will be applied.

---

# 🛠️ How to Edit the Translation (v2)

This is the guide for modifying the original files and creating your own custom translation using **UABEA**.

---

## 📋 Step by Step

1. **Open the file in UABEA**

   * Download [UABEA](https://github.com/nesrak1/UABEA?tab=readme-ov-file).
   * Locate the original translation file.
   * Make the necessary modifications in the **EN** language.

2. **Save and export the modified file**

   * After translating, save the final version.
   * Drag the modified file into the game’s root folder at the following path:

   ```
   /SarahsHouse_Data/StreamingAssets/aa/StandaloneWindows64/localization-string-tables-english(en)_assets_all.bundle
   ```

3. **Fix the CRC with AddressablesTools**

   * Download [AddressablesTools](https://github.com/nesrak1/AddressablesTools/releases).
   * Run the following command:

   ```bash
   dotnet Example.dll patchcrc /SarahsHouse_Data/StreamingAssets/aa/catalog.json
   ```

4. **Enjoy your translation! 🎉**

   * Now just run the game and enjoy your translated version.

---

## ⚠️ Important Tips

* Always **back up** the original file before modifying it.
* Work on a copy and keep the **Base Zone (v2)** intact.
* If something goes wrong, restore the original file from this folder.