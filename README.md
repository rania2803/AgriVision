# AgriVision: Deep CNNs for Wild Animal Surveillance in Farms

## Description:
The Farm Animal Detection and Notification System is a project designed to utilize an ESP32-CAM module, an FTDI programmer, and Python code to detect the presence of animals in a farm environment and notify the owner accordingly. The system employs computer vision techniques to analyze images captured by the ESP32-CAM and identify animals using object detection algorithms. Upon detection of specific animals, such as elephants, the system sends an SMS notification to the owner to alert them of the animal's presence.

## Components Used:*
1. **ESP32-CAM Module**: The ESP32-CAM is a versatile microcontroller module with built-in Wi-Fi and camera capabilities, making it suitable for capturing images in remote locations.
2. **FTDI Programmer**: The FTDI programmer is used for uploading code and communicating with the ESP32-CAM module.
3. **Python (Jupyter Notebook)**: Python code is used for image processing, object detection, SMS notification, and interaction with Firebase Storage.
4. **Arduino IDE**: The Arduino IDE is used for programming the ESP32-CAM module to serve images over HTTP.

##Installation and Running the Code:
1. **Hardware Setup**:
   - Connect the ESP32-CAM module to the FTDI programmer for programming and power.
   - Ensure that the ESP32-CAM module is properly configured and connected to the farm environment where animal detection is required.

2. **Software Setup**:
   - Install the necessary libraries and dependencies for Python code execution:
     
     pip install opencv-python-headless cvlib numpy requests pillow twilio firebase-admin
     
   - Ensure you have an active Twilio account and obtain the account SID, authentication token, and phone numbers for sending SMS notifications.
   - Set up a Firebase project and obtain the service account key JSON file for authentication.

3. **Upload Arduino Code**:
   - Open the Arduino IDE and upload the provided Arduino code to the ESP32-CAM module.
   - Make sure to set up the correct Wi-Fi credentials and IP address for accessing the camera images.

4. **Run Python Code**:
   - Execute the provided Python code (preferably in a Jupyter Notebook or Python script).
   - Ensure that the serviceAccountKey.json file is placed in the same directory as the Python script.
   - Modify the cam_ip variable in the Python script to match the IP address of your ESP32-CAM module.
   - Run the script and observe the output for animal detection and SMS notifications.

**Note**: Make sure all components are properly connected and configured before running the code. Adjustments may be necessary based on specific hardware configurations and project requirements.

## References:
- OpenCV: https://opencv.org/
- cvlib: https://github.com/arunponnusamy/cvlib
- Firebase: https://firebase.google.com/
- Twilio: https://www.twilio.com/
