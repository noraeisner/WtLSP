# wtLSP
Traditional periodograms suffer from gaps in the data. While we known that Fourier analysis requires uniformly sampled data, even techniques such as Lomb-Scargle (specifically designed to not require uniformly sampled data) lose SNR when there is missing data. One of the main problems is that any gaps (big or small) increase the noise floor due to the window function. 

While we started this project of with methods that were distinctly worse than Lomb Scargle (wtLS), we are starting to come up with reasonable solutions to address this ongoing problem in stellar (and perhaps other areas of) astrophysics. 

In particular, we are trying to address the fact that not all gaps (i.e. gaps of all sizes) should necessarily be treated using the same methodology. While in-painting or simple interpolation may be 'okay' for small gaps (is it ever truly okay to make up data?), this should never be done for larger gaps (what is that cuts-off). 

Original science case: Finding stellar pulsations and thus characterizing the star. 
Data: in this case we focus on TESS data - this data has lots of small and lots of large gaps.


## Authors:
- **Nora Eisner**
- **David W Hogg**

## License:
Copyright 2023 the authors. This code is licensed for re-use under the open-source *MIT License*.
See the file `LICENSE` for more details.
