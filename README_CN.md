# AutoUnzip

<div align="right">
  <a href="README_CN.md">
    <img src="https://img.shields.io/badge/Language-中文-blue?style=for-the-badge" height="35" alt="中文说明">
  </a>
</div>

An automated program that monitors a specified folder for all compressed archives and extracts them automatically.

<div align="center">
  <img width="336" height="390" alt="image" src="https://github.com/user-attachments/assets/f17d8522-267e-41c9-b14a-0f934171782a" />
  <img width="407" height="390" alt="image" src="https://github.com/user-attachments/assets/1e59609f-d439-46de-9842-35bfe5dd1531" />
</div>

> **Note:** The English version is machine-translated. Please take the Chinese version as the authoritative standard. Corrections are welcome!

### Introduction
An automated program that monitors specified folders for compressed archives and extracts them automatically. 

**Development Note:** This tool was created with the assistance of **Gemini 3**. The author is a beginner. If you see strange coding styles, that is expected. Feedback via Issues is welcome!

### Key Features
* **Folder Monitoring:** Set specific folders to watch. Archives are extracted instantly upon detection.
* **Password Book:** Automatically tries saved passwords for encrypted archives. Ideal for frequent downloads from the same source.
* **Smart Extraction:** Automatically creates a subfolder if the archive contains multiple files to keep your directory clean.
* **Threads:** Adjustable CPU thread usage for faster extraction.

### ⚠️ Warnings & Tips
1.  **Dependencies:** You must have [7-Zip](https://www.7-zip.org/) installed.
2.  **Portable Mode:** Do not move the `.exe` file out of its folder. Configuration is saved in a local `.json` file; moving the executable will cause data loss.
3.  **Strict Mode:** Keep this **ON** to avoid conflicts with temporary files created by download managers (like IDM, Aria2, BaiduNetdisk).
