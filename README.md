# Infant-Vitality-Watch
The project Infant Vitality Watch aims at helping doctors and hospital staff monitor newborn babies and reduce the infant mortality rate and any death 
caused due to lack of medical attention at the right time.

## Project Objectives
The project seeks to develop a monitoring system enabling remote supervision of infants, facilitating timely detection of health issues. We aim to provide the following features:
1.Vital parameters(Oxygen,Heart Rate, ECG) readings.
2. Using Deep learning model for future predictions of health parameter readings.
3. Alert Generation.
4. View many patients and their urgency on a single screen.

## Methodology
1. Dataset Collection - The dataset used in the present work is based on Non-Invasive Fetal ECG Arrhythmia Database (NIFEADB), obtained from Physionet Each ECG recording consists of six channels, out of which one is from the maternal chest (single lead) and the rest are from abdominal channels (five leads). This database contains 12 fetal arrhythmia and 14 normal rhythms, recorded from 26 subjects.
2. Data pre-processing – The ECG signals are filtered using a Normalized Least Mean Square (NLMS) adaptive filter with a step size of 0.1 to remove noise and artifacts. Additionally, 1D convolution with a standard wavelet, such as the Gaussian wavelet, is used for time-domain filtering. This enhances feature extraction from convoluted fetal ECG (f-ECG) signals for improved fetal arrhythmia detection and classification.
3. Feature Extraction - Followed by pre-processing, three features (F1−F3) i.e., mean, standard deviation, root mean square are extracted from the convoluted f-ECG signals.
4. Classification - The ANN model is employed to classify fetal arrhythmia using the pre-processed f-ECG signals. After extracting relevant features through 1D convolution and time-domain filtering, the ANN is trained on these features to accurately distinguish between normal and abnormal heart rhythms.



![Screenshot (492)](https://github.com/user-attachments/assets/8bb276b0-eadd-472d-8ae5-729faa2ab369)

## Hardware Used
1. ECG Module: The AD8232 is a low-power, single-lead heart rate monitoring module designed for ECG and other biopotential measurement applications, offering a compact solution for heart rate monitoring and cardiac signal conditioning.
2. Heart rate and SpO2 meter: The MAX30100 is an integrated pulse oximetry and heart-rate monitor sensor, combining LEDs and photodetectors for accurate, non-invasive measurement of blood oxygen saturation and heart rate.		
3. Temperature Sensor: The MLX90614 is a non-contact infrared temperature sensor capable of measuring the temperature of objects from a distance, providing accurate and reliable readings through its built-in signal processing unit. 
4. Node MCU: an open-source IoT platform based on the ESP8266 Wi-Fi module.						
5. Arduino UNO: a popular open-source microcontroller board based on the ATmega328P.					
6. 16X2 LCD Display: a basic, widely used alphanumeric screen capable of showing 16 characters per line on 2 lines.

   ![hardware](https://github.com/user-attachments/assets/aaa2f153-c661-4bb4-9b0b-68cdae85a18b)

