# HRV

## Scope of Project
Personal project to apply concepts from UW Madison ECE 203 and ECE 330.

Analyze ECG data from the [MIT-BIH Normal Sinus Rhythm Database](https://physionet.org/content/nsrdb/1.0.0/) with Python using the predeveloped package [wfdb](https://wfdb.readthedocs.io/en/latest/index.html) as well as custom code. Learn about HRV processing decisions from resources listed below.

### Resources
[Clifford Thesis](https://web.mit.edu/~gari/www/papers/GDCliffordThesis.pdf)

[HRV Signal Applications](https://ebookcentral.proquest.com/lib/wisc/reader.action?docID=1447662)  

[Dynamic Electrocardiography](https://onlinelibrary-wiley-com.ezproxy.library.wisc.edu/doi/pdfdirect/10.1002/9780470987483)

[Heart rate variability: Standards of measurement, physiological interpretation, and clinical use](https://academic.oup.com/eurheartj/article/17/3/354/485572)

### Steps
1) Import ECG data into Python
2) Time Domain Analysis 

    a) Find RR intervals using Pan and and Tompkin’s QRS detector
    
4) Frequency Domain Analysis

    a) Re-sample RR
    
    b) Fourier Transform
    
    c) PSD
    
5) Compare results with those [found here](https://neuropsychology.github.io/NeuroKit/functions/hrv.html).
