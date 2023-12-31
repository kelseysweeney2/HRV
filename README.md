# HRV

## Scope of Project
Personal project to apply concepts from UW Madison ECE 203 and ECE 330.

Analyze ECG data from the [MIT-BIH Normal Sinus Rhythm Database](https://physionet.org/content/nsrdb/1.0.0/) with Python/MATLAB using the predeveloped package [wfdb](https://wfdb.readthedocs.io/en/latest/index.html) as well as custom code. Learn about HRV processing decisions from resources listed below.

### Resources
[Clifford Thesis](https://web.mit.edu/~gari/www/papers/GDCliffordThesis.pdf)

[HRV Signal Signal Analysis: Clinical Applications](https://ebookcentral.proquest.com/lib/wisc/reader.action?docID=1447662)  

[Dynamic Electrocardiography](https://onlinelibrary-wiley-com.ezproxy.library.wisc.edu/doi/pdfdirect/10.1002/9780470987483)

[Heart rate variability: Standards of measurement, physiological interpretation, and clinical use](https://academic.oup.com/eurheartj/article/17/3/354/485572)

[Pan & Thompkins QRS detector](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=4122029)

[Hamilton & Thompkins QRS detector](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=4122227)

### Steps
1) Import ECG data 
2) Time Domain Analysis 

    a) Find RR intervals using Pan Thompkins QRS detector and calculate HRV using RMSSD or SDNN

    b) Evaluate Pan Thompkins QRS detector using LTI System Descriptions and Characteristics

        i) Difference Equation (computation)
       ii) Impulse Response (intuition)
       iii) Frequency Response (intuition)
       iv) System Function/Transfer Function (intuition)
       v) Causal
       vi) Time Invariant
       vii) Linear
       viii) BIBO Stable
    
3) Frequency Domain Analysis : HRV is composed of certain well-defined rhythms, which are related to different regulatory mechanism of cardiovascular control (attr HRV Signal Signal Analysis: Clinical Applications)

    a) Power Spectral Density Analysis

       i) DFT
       ii) FFT
       iii) Windowed Fourier Transform
    
4) Stretch Goal: Implement real time filters using live HR data
