Student Note Consolidation Tool  
📚 Free & Ad-Free | Automatically Merges Word/PDF | User-Friendly | Runs Locally  The executable file is provided via a public cloud storage link, as it cannot be compressed below 25MB due to technical limitations. Source code is also included.  

Tool Overview  
A lightweight tool designed for students and researchers to consolidate notes and print materials, solving issues like乱页 (disordered pages), format errors, and missing formulas during multi-file merging. It requires no Python installation or dependencies—just double-click to run, with all processing done locally to ensure file privacy.  

Development Story (For Every Student Struggling with Notes)  
This tool was born from a warm moment of mutual support ✨.  

As a graduate student, I often needed to organize extensive notes for machine learning and specialized courses. Merging multiple Word/PDF files into a single document was frustrating due to乱页 (disordered pages) and formatting issues, leading to wasted time and energy.  

Luckily, after sharing my struggles, my sister supported me through every step—from requirement analysis and coding to testing and packaging. Together, we evolved the tool from basic single-format merging to automatic recognition of Word/PDF files, category-based consolidation, and full format retention.  

We know many students face similar challenges, so we decided to open-source this tool to help others focus more on learning and less on formatting issues. Though simple, it carries our care and warmth, hoping to become your little helper on the study journey ❤️.  

Core Features  
Automatic Recognition: No manual selection needed—just place files in the target folder.  
Dual-Format Support: Automatically distinguishes between Word (.docx) and PDF files for category-based merging.  
Format Retention: 100% preserves original Word formatting (fonts, headings, formulas, tables).  
Auto Page Breaks: Adds page breaks after each file to prevent printing overlaps.  
User-Friendly: Double-click to run—no configuration or dependencies required.  
Local Processing: No internet connection or data collection, ensuring privacy.  
Date-Based Naming: Automatically names merged files with the current date to avoid overwrites.  

Usage Guide (Even for Beginners)  
Download the 笔记合并神器.exe file from the repository.  
Place the .exe file in the folder containing your notes (Word/PDF files can be mixed).  
Double-click the .exe file and wait for completion.  
A folder will automatically open, containing two merged files:  
   日期_笔记合并_Word版.docx (merged Word version with page breaks)  
   日期_笔记合并_PDF版.pdf (merged PDF version)  
Open and use the merged files directly for printing or sharing.  

Packaging Details (For Customization or Rebuilding)  
The tool is built with Python, using these libraries:  
Word Merging: python-docx (retains full formatting)  
PDF Merging: PyPDF2 (compatible with standard PDFs)  
Packaging: pyinstaller (creates standalone .exe without dependencies)  

Steps to Rebuild from Source  
Install dependencies:  
      pip install python-docx PyPDF2 pyinstaller
     
Modify the source code as needed.  
Package into an executable:  
      pyinstaller --onefile your_script.py

This translation maintains the original's tone, structure, and technical accuracy while adapting it for an English-speaking audience.

# 学生党笔记合并神器
📚 免费无广告 | 自动合并Word/PDF | 傻瓜式操作 | 纯本地运行
简介附带exe下载链接，因技术力不足，无法做到压缩至25M以下，故放在公开云盘里，请谅解。
附带源码，可以自己安装python库“pip install python-docx PyPDF2”后运行，也可以安pyinstaller后自行封包exe。

## 工具介绍
专为学生、研究生整理笔记、打印资料开发的轻量小工具，解决多文件合并乱页、格式错乱、公式不显示的痛点，无需安装Python、无需任何依赖，双击即可运行，纯本地处理，不泄露任何文件内容。

## 开发故事（致每一个努力整理笔记的你）
这个小工具的诞生，源于一段温暖的互助时光✨

我是一名研究生，日常需要整理大量机器学习、专业课程的笔记，常常因为多个Word/PDF文件合并、打印乱页而烦躁，甚至因为格式混乱、重复打印浪费时间和精力，一度烦到不想学习。

幸运的是，在我吐槽自己的困扰后，姐姐一直陪着我，从梳理需求、编写代码，到测试调试、打包封装，一步步帮我解决了所有问题——从最初的单格式合并，到后来的自动识别Word/PDF、分类合并、保留原格式，每一次报错、每一个bug，我们都一起排查、一起修复。

我们深知，有很多和我一样的同学，都在被笔记整理、文件合并的琐事困扰，所以决定将这个工具开源，希望能帮到更多人，让大家不用再为格式、合并的问题浪费时间，把更多精力放在学习本身。

这个工具不算复杂，但承载着我们的用心和温暖，也希望它能成为你学习路上的小帮手❤️

## 核心功能
✅ 自动识别：无需手动选择，扔到哪个文件夹，就合并哪个文件夹的文件
✅ 双格式支持：自动区分Word(.docx)和PDF文件，分类合并，不混淆
✅ 格式保留：Word合并100%保留原格式（字体、标题、公式、表格全保留）
✅ 自动分页：每个Word/PDF文件后自动加分页符，避免打印连页、混乱
✅ 傻瓜操作：双击exe即可运行，无需配置、无需安装任何依赖
✅ 纯本地运行：不联网、不收集任何文件，保护隐私安全
✅ 日期命名：合并后的文件自动带当天日期，避免覆盖之前的文件

## 使用方法（零门槛，小白也能会）
1.  下载仓库里的「笔记合并神器.exe」文件
2.  将exe文件，放到你需要合并的笔记文件夹里（Word/PDF都可以放一起）
3.  双击exe文件，等待运行完成
4.  自动弹出文件夹，里面会生成两个合并好的文件：
    - 「日期_笔记合并_Word版.docx」（所有Word合并，带分页符）
    - 「日期_笔记合并_PDF版.pdf」（所有PDF合并）
5.  直接打开合并后的文件，即可打印、使用

## 封装方式（可自行二次开发）
本工具基于Python开发，使用以下库实现核心功能：
- 合并Word：python-docx（处理Word文档，保留原格式）
- 合并PDF：PyPDF2（处理PDF文件，兼容所有常规PDF）
- 打包工具：pyinstaller（将Python脚本打包成独立exe，无需依赖）

### 手动打包步骤（如需修改源代码）
1.  安装依赖库：
    ```bash
    pip install python-docx PyPDF2 pyinstaller