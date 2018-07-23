# Data Input Cleaning and Encoding Library (DICE)

## Functionality:  
### data clean and resampling
1. data clean  
a. drop na row  
b. data imputation 

2. data resampling  
a. The input can be either one single file, multiple files or a folder.  
b. The output can be one single file or multiple files depending on the parameter setting 'output' which can be either s (single) or m (multiple). When m is selected, parameter granularity cannot be null. It has to be one of d (day), h (hour) or m (minute).

3. data resampling and merging  
a. Data resampling and merging at the same time. Data resampling as above.  
b. For data merging, the data need to have one anchor signal and one or more boat signals. The merging output file name should be assigned.  

### reliability check
1. For every step in the library, one reli_check parameter can be assigned as True or False. When True, a corresponding reliability file for each data file will be saved. File name and path will be assigned. 

### data encoding
1. Annotation file and data file are two inputs.
2. Label column(s) will be appended in the data file. 
3. Inplace parameter will be assigned as True or False. When False, the output file name will be assigned. 
4. Compensate time drift for sensor signal.
5. Refine annotation when mistake made during labeling. 

### (data visulization)

(To author: pyAudioAnalysis is an example illutrating how the library could be used finally: https://github.com/tyiannak/pyAudioAnalysis/wiki/3.-Feature-Extraction)
