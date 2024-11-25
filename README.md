# TapTime Standard Operating Procedure:

## Installation:
\begin{enumerate}
\item Download the TapTime.mlappinstall file onto your computer. As long as you have an active MATLAB subscription, this will be the only file you need.
    \begin{enumerate}
    \item Note: This app was built using MATLAB R2021B. While most functions used are fairly standard, if you’re running a much older version of MATLAB, you may run into some problems. If this is the case, you will need to upgrade to a newer version of MATLAB.
    \end{enumerate}
\item Open MATLAB and click the “Apps” tab at the top.
\item Click “Install App” and navigate to the TapTime.mlappinstall file that you downloaded. Once selected, MATLAB will install the app.
\item Now, in the list of apps, TapTime will always be available for you to use in the “My Apps” category unless you choose to uninstall it.
\end{enumerate}

## Usage
Before opening TapTime, it’s important to note that the outputs of TapTime are CSVs that are saved to a subdirectory called TapTimeOut, which is created by the tool relative to where you open the app. So, you will want to make sure you open TapTime in the same directory every time to ensure your files are always saved to the same location.
Once you open the app, you should be presented with the screen shown below:

The first thing you need to do is to select the audio file you will be playing for the participant. To do this, click “Choose File” and navigate to the audio file you want to use.
Note: TapTime is configured to search for wav files, but if you want to upload an mp3, you can select “All files” instead of “.wav” in your file explorer. However, this will allow you to select any file type. If you upload any file that is not recognized as an audio file, you will get an error.
Once you selected your file, you will see the “File Path” field update with the path of the file you selected. If TapTime was able to successfully read the audio file you selected, you will also see “Ready to Start Audio” in the “Program Status” field.
Note: The Program Status field is where you will see all updates that require your attention. For example, it can be used to tell you if there’s an error or when your files are successfully saved at the end.
Before you play the audio file, make sure your sound is on and the participant is fully ready. It is also a good idea to fill in the “Participant ID” and “Trial #” fields. This information is used to save the file under a unique name.
Note: If you need to reset, feel free to hit the “Stop” button. However, know that this is not a pause button. Hitting “Stop” will stop the audio and reset the trial. Once you press “G” again, the audio will play from the start, and if you did not save your data, it will be overwritten.
Once you’re ready to start, press the “G” key to start the audio. The participant(s) can tap along using the “A” key or the “L” key. The tool supports two people tapping at once. If you only have one participant at a time, they can use either the “A” key or the “L” key, as long as they continue using the same key for the entire trial.
The trial will end only once the “Stop” button is pressed or the audio is finished. Upon completion, press “Export P’x’ CSV” to save the data.
Make sure you keep an eye on the Program Status bar at the top. Once you click this button, it will either confirm that the data has been saved successfully or tell you that the file already exists, in which case you will need to increment the trial number for that participant.
The data saved is in a millisecond-from-start format. This means that as soon as the “G” key is pressed to start the audio, a millisecond-precision timer begins, enabling the recording of taps from the participant.
Example: If the participant claps exactly 1 second, 1.5 seconds, and 2 seconds after the start of the audio, the contents of the exported CSV will read: 
[1000, 1500, 2000]
Once the data is saved, you can either load a new audio file, repeat the experiment (with a different Trial #), or close the application.
If there are any questions or concerns related to TapTime, feel free to contact me! 
Contact info: Xavier Velez, xvelez6@gatech.edu