
[Portuguese](https://github.com/matheuspessole/MSOfficeSetup/blob/main/README_pt.md) | English

# INSTALLATION: MICROSOFT OFFICE

This guide provides a **step-by-step** walkthrough for installing Microsoft Office using Microsoft's official deployment tool.

---

## 📥 1. Downloading the files

Download the installation package from the link below and extract its contents to `C:\`:

- [Download MS Office Setup](https://github.com/matheuspessole/MS_Office_Setup/releases)

---

## ⚙️ 2. Installation procedure

> **Warning:** This procedure **does not guarantee Microsoft Office licensing**. A valid license is required to activate the product.

### Step 1 – Preparation

- Run the `officedeploymenttool_17328-20162` file.
- When prompted, select the folder where the files were extracted:
  ```
  C:\MS Office Setup
  ```

### Step 2 – Installation via Terminal

Open **Command Prompt (CMD)** as **Administrator** and run the following commands:

```cmd
:: Navigate to the installation folder
cd C:\MS Office Setup

:: Start the Office installation
Setup.exe /configure Configuração.xml
```

---

## 🌐 Changing the installation language (OPTIONAL)

If you want to install Office in another language, edit the **`Configuração.xml`** file before starting the installation.

Locate the following line:

```xml
<Language ID="pt-br"/>
```

Change the value of the `ID` attribute to your desired language.

### Examples

| Language | Code |
|----------|------|
| Portuguese (Brazil) | `pt-br` |
| English (United States) | `en-us` |
| Spanish | `es-es` |
| French | `fr-fr` |
| German | `de-de` |
| Italian | `it-it` |

> **Important:** After making the changes, save the `Configuração.xml` file and run the installation command again.

---

## 📝 Notes

- This repository contains only the files required to install Microsoft Office.
- The procedure uses Microsoft's official **Office Deployment Tool (ODT)**.
- The installation **does not activate** Office. A valid Microsoft license is required to use the product.
- If you want to install a different edition, architecture (32/64-bit), or language, simply modify the `Configuração.xml` file before installation.
