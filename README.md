# brainlib

for background, consult the following tutorials: [Pre-processing EEG data from consumer devices](http://blog.cosmopol.is/eeg/2015/06/26/pre-processing-EEG-consumer-devices.html), and [Building a simple BCI with a Neursosky MindWave](http://blog.cosmopol.is/eeg/2014/07/26/classifying-EEG-SVM.html)

## use

The main function you should use is
`makeFeatureVector (readings, bins)`
where `readings` is a list of lists, where each sub-list is 1024 raw values from the neurosky device. `bins` is a number of bins - 100 is a sane starting value here (see tutorials above for more details).

```python
import brainlib
brainlib.makeFeatureVector(readings, 100) 
```


