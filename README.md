# DataPreprocessing_ART_to_PPG
Data preprocessing code for AI model that receives ART signal and generates PPG signal  
Extract data from mimic iii waveform database

1. 12sec set
 - Dataset for training
 - Both ART and PPG consist of clean segments of 12sec

2. 40sec set
 - Dataset for validation
 - ART
   Don't look at the previous 25 sec. Clean signal in the last 15 sec
 - PPG
   previous 25 sec are a clean signal, and the last 15 sec are a noisy signal
 - sampling using 'Selecting_40sec_ValSet.ipynb' and then resampling using 'Resampleing_40sec_ValSet.ipynb'