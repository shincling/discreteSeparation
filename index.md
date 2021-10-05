## Discretization and Re-synthesis: an alternative method to solve the Cocktail Party Problem

### Abstract
Neural network based models have significantly improved the performance of speech separation with the input waveform from scenarios like the cocktail party. Prominent methods (e.g., frequency-domain and time-domain speech separation) usually build regression model to recover the ground-truth speech as much as possible, with the masking-based design and the signal-level loss criterion (e.g., MSE or SI-SNR). We propose here that the synthesis-based approach can also perform well towards this problem, with great flexibility and potential.  Specifically, we propose a novel speech separation/enhancement model based on the recognition of discrete symbols, converting the paradigm of the speech separation/enhancement related tasks from regression problem to classification task. By utilizing the synthesis model with the input of discrete symbols, after the prediction of discrete symbol sequence, each target speech could be re-synthesized. The experimental evaluation with the WSJ0-2mix and VCTK-noisy corpus in various settings shows that the proposed method could steadily synthesize the separated speech of good listening quality, nearly without any interference, which is difficult to avoid in regression based methods. In addition, with quite little loss of listening quality, the speaker conversion of enhanced/separated speech could be easily realized through our method.


### Test samples
Test wav1: https://github.com/shincling/discreteSparation/blob/gh-pages/wavs/clip0009_2_0.wav

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSparation/blob/gh-pages/wavs/clip0009_2_0.wav?raw=true">
</audio>

### Notice
This page is still under building, will be released soon.

