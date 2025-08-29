# 🪪 Student ID Card Generator
- Yo! This project lets you auto-generate a student ID card using Python + OpenCV.
- Basically: upload your pic, throw in your deets, and boom 💥 — you’ve got a fresh ID card saved as an image.

### ✨ Features
###### 📷 Drop in your passport photo (auto resized)
###### 🖊️ Add Name, ID, Role in style
###### 🎨 Borders + header line = instant card vibes
###### 💾 Save it forever as a .jpg

### 🛠️ Stack
##### 🐍 Python 3
##### 👀 OpenCV (pip install opencv-python)
##### 🔢 NumPy (pip install numpy)

### 🚀 How To Run
###### Clone repo
git clone https://github.com/your-username/id-card-generator.git
cd id-card-generator
###### Install reqs
pip install opencv-python numpy
###### Run it
python id_card.py

### 🧩 How It Works
- Loads a blank ID card (or template).
- Pastes your photo at fixed coordinates.
- Draws a photo border box.
- Adds your:
  - 🏷️ Name
  - 🔢 ID Number
  - 🎓 Role
- Slaps on an institution name + footer line.
- Saves output as student_id_card.jpg.

### 📍 Coordinate Cheat Sheet
###### - Element	Old Value	New Value (200×180 photo)
###### - Resize (photo)	(150,180)	(200,180)
###### - Paste Range	[50:230,50:200]	[50:230,50:250]
###### - Rectangle Border	(50,50),(210,240)	(50,50),(250,240)

### 💡 Customizing
- Change photo size → tweak cv2.resize()
- Shift text → edit (x, y) values in cv2.putText()
- Update org name → replace "University of Mumbai"
