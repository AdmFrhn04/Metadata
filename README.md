# Metadata
TASK W4 VA

**Tools learned:**
1. `file`
2. `strings`
3. `exiftool`
4. `hexeditor`
5. `binwalk`

## Task

| Picture        | Tools             | Link / Command       | POC  | Analysis |
|----------------|-------------------|----------------------|------|----------|
| Ocean.jpg      | exiftool          | https://exif.tools/  | <img width="1909" height="943" alt="Screenshot 2026-04-15 034636" src="https://github.com/user-attachments/assets/f1804d47-5364-4871-83aa-e82e211ed4b6" /> | Online tools can also output same result as command in Kali. Many online tools are actually built using the same underlying engines found in Kali Linux, specifically ExifTool.          |
|                |                   | `exiftool ocean.jpg` | <img width="587" height="625" alt="Image" src="https://github.com/user-attachments/assets/9361ed00-6a81-4e35-9ffd-89f91f35ae1b" /> | Can clearly saw the flag in comment section          |
| Computer.jpg   | Hexeditor         | https://hexed.it/    | <img width="1910" height="945" alt="Screenshot 2026-04-15 040448" src="https://github.com/user-attachments/assets/9671884d-1ee0-47bd-b866-0e3ab47295df" />| Analyse the docs header      |
|                |                   | `hexeditor computer.jpg` | <img width="881" height="191" alt="Image" src="https://github.com/user-attachments/assets/bbb7695a-b306-420e-ae6b-a28a744bfcb8" />  | Hexeditor in kali is really easy to use. <br> Can refer here for the header https://filesig.search.org/ |
| dog.jpg        | binwalk           | `binwalk dog.jpg` <br> `binwalk -e dog.jpg` <br> `cd _dog.jpg.extracted/` | <img width="983" height="445" alt="Image" src="https://github.com/user-attachments/assets/44b94fea-eb24-4f7f-984e-98553339e079" /> | `binwalk` usually use for finding hidden file in the main file  |
| computer.jpg   | strings           | https://www.dcode.fr/strings-extractor | <img width="1914" height="943" alt="Screenshot 2026-04-15 040655" src="https://github.com/user-attachments/assets/00324fdf-db42-49fd-b940-c11428886a8c" />| online tools for command `strings` |
|                |                   | `strings computer.jpg`| <img width="285" height="252" alt="Image" src="https://github.com/user-attachments/assets/6656a25e-96b2-4ce8-8125-b58482b3c65e" />  | used to extract human-readable text from files, especially binary files.          |
| solitaire.exe  | file | `file solitaire.exe` | <img width="535" height="51" alt="Image" src="https://github.com/user-attachments/assets/d9b3d678-9064-45ef-80dc-b81fd8235f98" /> | solitare.exe is actually a PNG file |
| rubiks.jpg     | file | `file rubiks.jpg`    | <img width="511" height="50" alt="Image" src="https://github.com/user-attachments/assets/fd42fc35-9ca2-441b-a80b-1f8dd695f9ac" /> | After checking the jpg file is actually a png |
