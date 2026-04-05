📚 学生党笔记合并神器 - 使用须知

一款专为学生党设计的轻量化笔记合并工具，支持自动合并文件夹内所有Word（.docx）和PDF文件，无需手动操作，一键生成合并文件，适配日常笔记整理、复习资料汇总场景，简单好上手！

✨ 核心功能

- 自动识别：双击运行，自动定位脚本/EXE所在文件夹，无需手动选择路径

- 双格式合并：同时支持Word（.docx）和PDF文件合并，分别生成独立合并文件

- 格式保留：Word合并时100%保留原文件字体、样式、表格，无需重新排版

- 友好提示：弹窗提示操作结果（成功/失败），自动打开目标文件夹，一目了然

- 防错处理：自动跳过临时文件（如Word临时文件~$开头）、已合并文件，避免重复合并；文件被占用时弹窗提示

📖 基础使用方法（超简单！）

1. 准备工作：将需要合并的 Word（.docx） 或 PDF 文件，全部放到同一个文件夹中

2. 运行工具：将脚本（.py）或打包后的EXE文件，放到上述文件夹中，双击运行

3. 等待完成：工具自动筛选文件、执行合并，合并完成后会弹窗提示，并自动打开文件夹

4. 查看结果：文件夹中会生成两个合并文件（若只有一种格式，只生成对应文件）：
        

  - Word版：{日期}_笔记合并_Word版.docx

  - PDF版：{日期}_笔记合并_PDF版.pdf

🔍 关键说明：文件排序规则（重点！）

工具默认采用 按文件名排序（优先推荐，适配学生笔记整理场景），排序逻辑如下，建议配合规范命名使用，避免顺序混乱：

1. 排序优先级（从先到后）

数字（0-9） → 大写英文字母（A-Z） → 小写英文字母（a-z） → 汉字

2. 具体排序细节

- 数字：按「逐位字符对比」排序（非数字大小），示例：000 < 001 < 010 < 1 < 10 < 2

- 字母：大写优先于小写，示例：Apple < Banana < apple < banana

- 汉字：按拼音首字母排序（非笔画），示例：安 < 北 < 东 < 中

3. 为什么不选「按修改时间排序」？

笔记整理场景中，修改旧笔记会导致文件修改时间更新，进而打乱原有笔记顺序（比如4月4日的笔记，修改后会被排到4月5日笔记后面），因此按文件名排序更稳定，顺序永久固定，怎么修改文件都不会乱。

📌 推荐笔记命名规范（必看！）

配合按文件名排序，建议采用「日期+内容」的命名格式，顺序永远整齐，适配复习逻辑：

20260401_机器学习笔记.docx
20260402_结构力学笔记.docx
20260403_错题整理.pdf
20260404_英语单词总结.docx

优点：日期从小到大排序，复习时按时间线推进，且修改文件后，顺序不会改变。

❌ 常见问题及解决方法

- 问题1：提示“文件已被打开，请关闭后重试”

- 解决：关闭对应格式的合并文件（如已打开的Word/PDF合并文件），重新运行工具即可。

- 问题2：未找到可合并的文件

- 解决：检查文件夹内文件格式是否为 .docx（Word）或 .pdf（PDF），且未被重命名为“合并文件”格式。

- 问题3：Word合并后格式错乱

- 解决：确保原Word文件格式正常（无损坏），工具会自动保留原格式，无需额外操作。

- 问题4：PDF合并失败

- 解决：检查PDF文件是否损坏、加密，加密或损坏的PDF无法正常合并。

💡 小技巧

- 若只想合并一种格式（如只合并Word），只需将另一种格式文件移出文件夹即可。

- 打包成EXE后，可直接放在任意笔记文件夹中运行，无需安装Python环境。

- 合并后的Word文件，每个原文件之间会自动加分页符，便于区分不同笔记。

❤️ 致谢

本工具为自用笔记整理而生，简化学生党合并笔记的繁琐操作，感谢每一位使用的小伙伴～ 如有优化建议，欢迎留言交流！

📚 Student Notes Merge Tool - Usage Guide  

A lightweight notes merge tool designed specifically for students, supporting automatic merging of all Word (.docx) and PDF files in a folder. No manual operation is required—just one click to generate a merged file. It is suitable for daily notes organization and review material compilation, with a simple and user-friendly interface.  

✨ Core Features  

Automatic Recognition: Double-click to run; the tool automatically locates the folder where the script/EXE is placed, no need to manually select a path.  
Dual-Format Merging: Supports merging both Word (.docx) and PDF files, generating separate merged files for each format.  
Format Preservation: 100% retains original fonts, styles, and tables when merging Word files—no reformatting needed.  
User-Friendly Prompts: Popup notifications for operation results (success/failure), and automatically opens the target folder for easy access.  
Error Prevention: Automatically skips temporary files (e.g., Word temp files starting with ~$) and already merged files to avoid duplication; prompts if a file is in use.  

📖 Basic Usage (Super Simple!)  

Preparation: Place all Word (.docx) or PDF files to be merged into the same folder.  
Run the Tool: Place the script (.py) or packaged EXE file into the same folder and double-click to run.  
Wait for Completion: The tool automatically filters files and performs the merge. A popup will notify you upon completion, and the folder will open automatically.  
View Results: The folder will contain two merged files (only one file will be generated if only one format is present):  
   Word Version: {date}_NotesMerge_WordVersion.docx  
   PDF Version: {date}_NotesMerge_PDFVersion.pdf  

🔍 Key Note: File Sorting Rules (Important!)  

The tool uses file name sorting by default (recommended for student notes organization). The sorting logic is as follows—use standardized naming to avoid order confusion:  

Sorting Priority (from highest to lowest)  
   Numbers (0-9) → Uppercase English letters (A-Z) → Lowercase English letters (a-z) → Chinese characters  

Detailed Sorting Rules  
   Numbers: Sorted by character-by-character comparison (not numerical value), e.g., 000 < 001 < 010 < 1 < 10 < 2.  
   Letters: Uppercase comes before lowercase, e.g., Apple < Banana < apple < banana.  
   Chinese Characters: Sorted by pinyin initial letter (not stroke count), e.g., 安 < 北 < 东 < 中.  

Why Not Sort by Modification Time?  
   In notes organization, modifying old notes updates the file modification time, which can disrupt the original order (e.g., a note from April 4 might be placed after April 5 notes after modification). File name sorting is more stable—the order remains fixed, regardless of file modifications.  

📌 Recommended Naming Convention (Must Read!)  

To align with file name sorting, use a date + content naming format to keep your notes in perfect order, matching your review logic:  

20260401_MachineLearningNotes.docx
20260402_StructuralMechanicsNotes.docx
20260403_ErrorCollection.pdf
20260404_EnglishVocabularySummary.docx
  

Advantages:  
Dates sorted from earliest to latest, allowing you to review in chronological order.  
File modifications will not change the order.  

❌ Common Issues & Solutions  

Issue 1: "File is already open, please close and retry."  
  Solution: Close the merged file (Word/PDF) that is currently open, then rerun the tool.  

Issue 2: "No mergeable files found."  
  Solution: Check if the files in the folder are in .docx (Word) or .pdf (PDF) format, and ensure they are not renamed to match the merged file format.  

Issue 3: "Word merge results in formatting issues."  
  Solution: Ensure the original Word files are not corrupted—the tool automatically preserves the original format.  

Issue 4: "PDF merge fails."  
  Solution: Check if the PDF files are damaged or encrypted—encrypted or damaged PDFs cannot be merged.  

💡 Pro Tips  

If you want to merge only one format (e.g., only Word), simply move the other format files out of the folder.  
After packaging into an EXE, you can place it directly in any notes folder and run it—no Python environment required.  
The merged Word file will automatically insert page breaks between original files, making it easy to distinguish different notes.  

❤️ Acknowledgements  

This tool was created to simplify my own notes organization, aiming to streamline the tedious process of merging notes for students. Thank you to everyone who uses it! If you have suggestions for improvement, feel free to share them.
