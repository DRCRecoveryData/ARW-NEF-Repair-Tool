# ARW/NEF-Repair-Tool

![image](https://github.com/DRCRecoveryData/ARW-NEF-Repair-Tool/blob/main/Images/Screenshot%20from%202024-04-29%2017-42-00.png)

ARW/NEF-Repair-Tool is a PyQt6 application for repairing ARW/NEF image files using a reference ARW/NEF file. Provides a user-friendly GUI.

## Demo

![Watch the video]()

## Requirements

- Python 3.x
- PyQt6
- Rawpy
- imageio

```pip install pyqt6 rawpy imageio```
  
## Usage

1. Clone the repository or download the `arwnefrepair-gui.py` file.
2. Install PyQt6 if you haven't already:
    ```
    pip install PyQt6
    ```

4. Run the `arwnefrepair-gui.py` file:
    ```
    python arwnefrepair-gui.py
    ```
5. The GUI window will appear. Use the "Browse" buttons to select the reference ARW/NEF file and the encrypted folder.
6. Click the "Repair" button to start the repair process.
7. Progress will be displayed in the progress bar and log box. Once the repair is complete, a success message will appear.

## How it Works

- The tool reads the reference ARW/NEF file and locates the offset header.
- It then scans the encrypted folder for ARW/NEF files to be repaired.
- For each file found, it copies the data after the offset header from the reference file and writes it to a new file in the "Repaired" folder.
- The process is tracked in the log box, and progress is shown in the progress bar.

## Styling

- The GUI features modern blue buttons styled with CSS to enhance the user experience.

## Limitations

- This tool is specifically designed for repairing ARW/NEF files and may not work with other file formats.
- It assumes that the reference ARW/NEF file and the encrypted files have a specific structure, so results may vary with different files.

## Disclaimer

- Use this tool at your own risk. Always make backups of your files before attempting any modifications.
