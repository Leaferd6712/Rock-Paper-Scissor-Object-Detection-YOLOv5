Rock Paper Scissors Object Detection using YOLOv5
- The Object Detection Model is Pretrained (no need to train on your device)
- This project uses YOLOv5 and computer vision to detect Rock, Paper, and Scissors hand gestures in real time using your webcam
- These instructions are for Windows using PowerShell
- Adjust code for Linux/Apple

Dataset:
(https://universe.roboflow.com/mathias-p/rock-paper-scissors-y8qwz)

Requirements:
- Python 3.8 or newer
- Git
- A webcam

Enter this to confirm your python version!
Enter THIS:
python --version



FULL SETUP GUIDE (STEP BY STEP)

Step 1 - Open PowerShell

On Windows:
Press Windows key + X, then click Terminal



Step 2 - Clone the Repository

Enter THIS:
git clone [https://github.com/Leaferd6712/Rock-Paper-Scissor-Object-Detection-YOLOv5.git](https://github.com/Leaferd6712/Rock-Paper-Scissor-Object-Detection-YOLOv5.git)

Enter THIS:
cd Rock-Paper-Scissor-Object-Detection-YOLOv5

Step 3 - How To Find Your Folder Path

If you ever need to find the full path of your project folder:

On Windows:
Method 1:

Open File Explorer

Go to the folder

Click the address bar

Copy the path

Method 2:

Hold Shift

Right-click the folder

Click "Copy as path"

Then in PowerShell:

Enter THIS:
cd "PASTE_THE_PATH_HERE"

Step 4 - Create a Virtual Environment (Only Once)

Make sure you are inside the project folder first.

Enter THIS:
python -m venv yolovenv

Step 5 - Activate the Virtual Environment

On Windows (PowerShell):

Enter THIS:
.\yolovenv\Scripts\Activate.ps1

If it worked, you should see (yolovenv) in the terminal.

If PowerShell blocks it:

Enter THIS:
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned

Then try again:

Enter THIS:
.\yolovenv\Scripts\Activate.ps1

Step 6 - Install Dependencies

Enter THIS:
pip install -r requirements.txt

Step 7 - Go To Your Actual Project Folder

Your project folder is located at:

C:\Users\mcmat\Documents\Optimised_Rock_Paper_Scissors

Enter THIS:
cd "C:\Users\mcmat\Documents\Optimised_Rock_Paper_Scissors"

(Use the copy path method above to get the correct path.)

Step 8 - Run the Rock Paper Scissors Detector

Enter THIS:
python detect.py --weights runs/train/third_run/weights/best.pt --source 0 --img-size 640 --conf-thres 0.25 --device 0

What this does:

Opens your webcam

Uses your trained YOLOv5 model

Detects Rock, Paper, Scissors in real time

How to run it again next time:

Enter THIS:
cd "YOUR_PROJECT_FOLDER_PATH"

Enter THIS:
Activate the virtual environment again (same command as Step 5)

Enter THIS:
python detect.py --weights runs/train/third_run/weights/best.pt --source 0 --img-size 640 --conf-thres 0.25 --device 0

Author:
Mathias

License:
This project is for educational purposes only.

---

If you want, I can also make a **short “Quick Start” version** for the top of the README.
