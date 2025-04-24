# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
Name:Vimala Rani A

Reg No:212223040240
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.

## DESIGN STEPS:
### Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

### Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

### Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

## PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps
# A. Using ExifTool – for file metadata

 Install:

sudo apt update
sudo apt install exiftool -y

 Extract metadata from a file:

exiftool image.jpg

 Batch process a folder:

exiftool -r /path/to/folder

Useful flags:

-G: Show metadata group

-time:all: Show only timestamps

-GPSLatitude -GPSLongitude: Extract GPS data

![Screenshot 2025-04-24 233155](https://github.com/user-attachments/assets/0fc6ba3b-c9d3-4f88-ada8-f316c7c79112)


# install log2timeline

sudo apt install plaso -y


sudo apt install steghide -y

# Embed data

steghide embed -cf /home/kali/Downloads/wallpaper.jpg -ef /home/kali/Downloads/secret.txt

![Screenshot 2025-04-24 233304](https://github.com/user-attachments/assets/8e49a566-490a-431b-bf17-de174583b775)


Extract hidden data:

steghide extract -sf hidden.jpg

![Screenshot 2025-04-24 233314](https://github.com/user-attachments/assets/ceadc246-6e74-4f26-9ecd-e9bd253d24dd)


# Using binwalk – for file analysis


sudo apt install binwalk -y
binwalk suspicious.jpg

![Screenshot 2025-04-24 233322](https://github.com/user-attachments/assets/7f796822-db61-4d83-b54d-bae7796934d0)


## OUTPUT:
Extracted Metadata, Timeline Events, and Hidden Data Detection Results
![Screenshot 2025-04-24 233345](https://github.com/user-attachments/assets/3ddbd671-39fe-45e1-961a-ad849d2c11e5)


## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.
