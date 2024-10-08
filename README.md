# Plotting Sinusoidal Wave in LabVIEW

This LabVIEW project contains two files, `Sin.vi` and `Sin обр.vi`, which demonstrate plotting a sinusoidal wave on a waveform chart. Both VIs showcase how to generate and display a sine wave, with a slight variation in the user input control between the two files.

## Overview

- **`Sin.vi`**:  
  This VI generates a basic sine wave and plots it on a waveform chart. The user initiates the plotting by pressing the "Start" button, and the sine wave is calculated based on the degree input.

- **`Sin обр.vi`**:  
  This VI is similar to `Sin.vi`, but includes an additional numeric control that allows the user to modify the degree input dynamically. The waveform chart updates based on the changes in both the "Start" button and the numeric value.

## Features

### Sin.vi

1. **Start Button Trigger**:  
   The waveform plotting starts when the user presses the "Start" button.
   
2. **Waveform Chart**:  
   The program converts degree input into radians using the formula:
   ```plaintext
   radians = degrees * π / 180
   ```
   and then generates a sine wave, which is plotted on the chart.

3. **Continuous Update**:  
   The chart continuously updates the sine wave based on the internal iteration in a while loop, until the "Stop" button is pressed.

### Sin обр.vi

1. **Start Button Trigger**:  
   Similar to `Sin.vi`, the plotting begins when the user presses the "Start" button.
   
2. **Numeric Input Control**:  
   In addition to the start button, the user can modify the degree input dynamically via the numeric control. Any changes to the numeric value immediately affect the plot on the waveform chart.

3. **Waveform Chart**:  
   The chart plots the sine wave, updating continuously with the new values entered in the numeric control.

## How It Works

- **Sinusoidal Plotting**:  
  Both VIs convert the degree input to radians and use the LabVIEW `Sin` function to generate sine wave values.
  
- **Event Structure**:  
  The event structure captures user interactions such as pressing the "Start" button or modifying the numeric value (in `Sin обр.vi`), ensuring real-time updates to the plot.

- **Waveform Chart**:  
  The results are displayed on a waveform chart, with the x-axis representing the degrees and the y-axis showing the sine of the corresponding angles.

## Usage

- Run `Sin.vi` or `Sin обр.vi`.
- Press the "Start" button to begin plotting the sine wave.
- In `Sin обр.vi`, modify the numeric control to see the waveform chart update in real-time.
- Press the "Stop" button to stop the plotting process.

## Requirements

- LabVIEW software is required to open and run these VIs.



## Sin.vi
### Code
![image](https://github.com/user-attachments/assets/9fb78c99-0d29-421c-a8cd-e86ca7acc54e)

### The appearance of the running program
![image](https://github.com/user-attachments/assets/5afd196f-5db7-4214-95a6-f58bbe799401)

## Sin обр.vi - Numeric from 0 to 1 floating point truncates sin.
### Code
![image](https://github.com/user-attachments/assets/42b58e59-da5e-443f-9fb3-2a2dbb884086) 
![image](https://github.com/user-attachments/assets/779ea1e3-428e-4f47-b796-9ad3f5166644) 
![image](https://github.com/user-attachments/assets/3d974490-dd20-4f52-ba66-be8466cc2ae9)

### The appearance of the running program
![image](https://github.com/user-attachments/assets/52d0ac8c-1b92-4414-bc84-54637f9af3b9)
![image](https://github.com/user-attachments/assets/416a8c31-b1bf-4945-aa24-f9a43803f241)
![image](https://github.com/user-attachments/assets/ff342598-fc7f-4b83-8b94-8bf59338fb8e)
