## Discretization and Re-synthesis: an alternative method to solve the Cocktail Party Problem

### Abstract
Neural network based models have significantly improved the performance of speech separation with the input waveform from scenarios like the cocktail party. Prominent methods (e.g., frequency-domain and time-domain speech separation) usually build regression model to recover the ground-truth speech as much as possible, with the masking-based design and the signal-level loss criterion (e.g., MSE or SI-SNR). We propose here that the synthesis-based approach can also perform well towards this problem, with great flexibility and potential.  Specifically, we propose a novel speech separation/enhancement model based on the recognition of discrete symbols, converting the paradigm of the speech separation/enhancement related tasks from regression problem to classification task. By utilizing the synthesis model with the input of discrete symbols, after the prediction of discrete symbol sequence, each target speech could be re-synthesized. The experimental evaluation with the WSJ0-2mix and VCTK-noisy corpus in various settings shows that the proposed method could steadily synthesize the separated speech of good listening quality, nearly without any interference, which is difficult to avoid in regression based methods. In addition, with quite little loss of listening quality, the speaker conversion of enhanced/separated speech could be easily realized through our method.


### Test samples
#### Female + Female

(1) Sample1: 

Mixture Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/Mix/053_444_053a050p_1.912_444o030g_-1.912.wav?raw=true">
</audio>

Conv-TasNet:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/ConvTasNet/053_444_053a050p_1.912_444o030g_-1.912_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/ConvTasNet/053_444_053a050p_1.912_444o030g_-1.912_pre2.wav?raw=true"></audio>

Conv-DPRNN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/DPRNN/053_444_053a050p_1.912_444o030g_-1.912_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/DPRNN/053_444_053a050p_1.912_444o030g_-1.912_pre2.wav?raw=true"></audio>

Our discrete Separation:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/053_444_053a050p_1.912_444o030g_-1.912_pre1.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/053_444_053a050p_1.912_444o030g_-1.912_pre2.wav?raw=true"></audio>

(2) Sample2: 

Mixture Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/Mix/420_053_420a0104_0.4599_053o020i_-0.4599.wav?raw=true">
</audio>

Conv-TasNet:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/ConvTasNet/420_053_420a0104_0.4599_053o020i_-0.4599_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/ConvTasNet/420_053_420a0104_0.4599_053o020i_-0.4599_pre2.wav?raw=true"></audio>

Conv-DPRNN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/DPRNN/420_053_420a0104_0.4599_053o020i_-0.4599_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/DPRNN/420_053_420a0104_0.4599_053o020i_-0.4599_pre2.wav?raw=true"></audio>

Our discrete Separation:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/420_053_420a0104_0.4599_053o020i_-0.4599_pre1.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/420_053_420a0104_0.4599_053o020i_-0.4599_pre2.wav?raw=true"></audio>

(3) Sample3: 

Mixture Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/Mix/420_444_420a0114_0.39756_444o0314_-0.39756.wav?raw=true">
</audio>

Conv-TasNet:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/ConvTasNet/420_444_420a0114_0.39756_444o0314_-0.39756_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/ConvTasNet/420_444_420a0114_0.39756_444o0314_-0.39756_pre2.wav?raw=true"></audio>

Conv-DPRNN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/DPRNN/420_444_420a0114_0.39756_444o0314_-0.39756_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/DPRNN/420_444_420a0114_0.39756_444o0314_-0.39756_pre2.wav?raw=true"></audio>

Our discrete Separation:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/420_444_420a0114_0.39756_444o0314_-0.39756_pre1.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FF/420_444_420a0114_0.39756_444o0314_-0.39756_pre2.wav?raw=true"></audio>



### Notice
This page is still under building, will be released soon.

