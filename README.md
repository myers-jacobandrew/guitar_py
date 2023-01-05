# guitar_py

This code is intended to be used to detect the pitch of an audio signal from an input in real-time. 

It uses PyAudio to handle the audio recording and Librosa to detect the pitch of the audio signal. The user is prompted to select an input device, and then the audio signal is plotted in a Matplotlib figure along with an estimate of the pitch in Hz. The pitch detection is done using a function called detect_pitch_librosa which converts the audio data to a waveform and then runs the pitch detection algorithm from Librosa on the waveform. The pitch is then estimated as the mean pitch of the highest energy frames. The code also includes a function called check_sample_rate which checks whether the user-specified sample rate is compatible with the selected input device, and prompts the user to confirm whether they want to switch to the default sample rate of the device if necessary.
