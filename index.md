# Discretization and Re-synthesis: an alternative method to solve the Cocktail Party Problem
## Abstract
Neural network based models have significantly improved the performance of speech separation with the input waveform from scenarios like the cocktail party. Prominent methods (e.g., frequency-domain and time-domain speech separation) usually build regression model to recover the ground-truth speech as much as possible, with the masking-based design and the signal-level loss criterion (e.g., MSE or SI-SNR). We propose here that the synthesis-based approach can also perform well towards this problem, with great flexibility and potential.  Specifically, we propose a novel speech separation/enhancement model based on the recognition of discrete symbols, converting the paradigm of the speech separation/enhancement related tasks from regression problem to classification task. By utilizing the synthesis model with the input of discrete symbols, after the prediction of discrete symbol sequence, each target speech could be re-synthesized. The experimental evaluation with the WSJ0-2mix and VCTK-noisy corpus in various settings shows that the proposed method could steadily synthesize the separated speech of good listening quality, nearly without any interference, which is difficult to avoid in regression based methods. In addition, with quite little loss of listening quality, the speaker conversion of enhanced/separated speech could be easily realized through our method.


## Test samples of Speech enhancement 
The sound files blow are some raw noisy wavs and the enhanced speech from different methods.
All the samples are driven from the test set of VCTK-noisy.

Notice: here we use the vctk vocoder or the ljspeech vocoder. The former one corresponds to the training corpus we used (vctk-noisy) while the later one is an external single-speaker corpus, which could be used to show the speaker-transfer characteristic of our method.

**(1) Sample1:** 

Noisy Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/noisy/p232_072.wav?raw=true"></audio>

Conv-TasNet:           MTL-mimic-voicebank:              
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/ConvTasNet/p232_072.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/mtl/p232_072.wav?raw=true"></audio>
Metricgan-voicebank:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/metricgan/p232_072.wav?raw=true"></audio>
Our discrete enhancement (with vctk vocoder /  ljspeech vocoder):
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/p232_072.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/our_ljspeech_vocoder/p232_072.wav?raw=true"></audio>

**(2) Sample2:** 

Noisy Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/noisy/p232_156.wav?raw=true"></audio>

Conv-TasNet:           MTL-mimic-voicebank: 
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/ConvTasNet/p232_156.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/mtl/p232_156.wav?raw=true"></audio>

Metricgan-voicebank:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/metricgan/p232_156.wav?raw=true"></audio>

Our discrete enhancement (with vctk vocoder /  ljspeech vocoder):
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/p232_156.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/our_ljspeech_vocoder/p232_156.wav?raw=true"></audio>

**(3) Sample3:** 

Noisy Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/noisy/p232_378.wav?raw=true"></audio>

Conv-TasNet:           MTL-mimic-voicebank:  
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/ConvTasNet/p232_378.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/mtl/p232_378.wav?raw=true"></audio>

Metricgan-voicebank:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/metricgan/p232_378.wav?raw=true"></audio>

Our discrete enhancement (with vctk vocoder /  ljspeech vocoder):
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/p232_378.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/our_ljspeech_vocoder/p232_378.wav?raw=true"></audio>


**(4) Sample4:** 

Noisy Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/noisy/p232_383.wav?raw=true"></audio>

Conv-TasNet:           MTL-mimic-voicebank:  
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/ConvTasNet/p232_383.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/mtl/p232_383.wav?raw=true"></audio>

Metricgan-voicebank:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/metricgan/p232_383.wav?raw=true"></audio>

Our discrete enhancement (with vctk vocoder /  ljspeech vocoder):
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/p232_383.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/our_ljspeech_vocoder/p232_383.wav?raw=true"></audio>

**(5) Sample5:** 

Noisy Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/noisy/p257_046.wav?raw=true"></audio>

Conv-TasNet:           MTL-mimic-voicebank:  
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/ConvTasNet/p257_046.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/mtl/p257_046.wav?raw=true"></audio>

Metricgan-voicebank:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/metricgan/p257_046.wav?raw=true"></audio>

Our discrete enhancement (with vctk vocoder /  ljspeech vocoder):
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/p257_046.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/our_ljspeech_vocoder/p257_046.wav?raw=true"></audio>

**(6) Sample6:** 

Noisy Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/noisy/p257_335.wav?raw=true"></audio>

Conv-TasNet:           MTL-mimic-voicebank:  
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/ConvTasNet/p257_335.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/mtl/p257_335.wav?raw=true"></audio>

Metricgan-voicebank:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/metricgan/p257_335.wav?raw=true"></audio>

Our discrete enhancement (with vctk vocoder /  ljspeech vocoder):
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/p257_335.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/our_ljspeech_vocoder/p257_335.wav?raw=true"></audio>

**(7) Sample7:** 

Noisy Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/noisy/p257_412.wav?raw=true"></audio>

Conv-TasNet:           MTL-mimic-voicebank:  
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/ConvTasNet/p257_412.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/mtl/p257_412.wav?raw=true"></audio>

Metricgan-voicebank:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/metricgan/p257_412.wav?raw=true"></audio>

Our discrete enhancement (with vctk vocoder /  ljspeech vocoder):
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/p257_412.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs_vctk/our_ljspeech_vocoder/p257_412.wav?raw=true"></audio>


## Test samples of Speech separation 
The sound files blow are some raw mixture wavs and the separated speech from different methods.
We show the different gender combination results as: Female+Female / Female+Male/ Male+Male.
All the samples are driven from the test set of WSJ0-2mix.

### Female + Female

**(1) Sample1:** 

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

**(2) Sample2:**  

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

**(3) Sample3:** 

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

### Female + Male

**(1) Sample1:** 

Mixture Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/Mix/053_423_053o0206_0.66993_423a0105_-0.66993.wav?raw=true">
</audio>

Conv-TasNet:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/ConvTasNet/053_423_053o0206_0.66993_423a0105_-0.66993_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/ConvTasNet/053_423_053o0206_0.66993_423a0105_-0.66993_pre2.wav?raw=true"></audio>

Conv-DPRNN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/DPRNN/053_423_053o0206_0.66993_423a0105_-0.66993_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/DPRNN/053_423_053o0206_0.66993_423a0105_-0.66993_pre2.wav?raw=true"></audio>

Our discrete Separation:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/053_423_053o0206_0.66993_423a0105_-0.66993_pre1.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/053_423_053o0206_0.66993_423a0105_-0.66993_pre2.wav?raw=true"></audio>

**(2) Sample2:** 

Mixture Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/Mix/051_444_051c0101_1.9809_444o030u_-1.9809.wav?raw=true">
</audio>

Conv-TasNet:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/ConvTasNet/051_444_051c0101_1.9809_444o030u_-1.9809_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/ConvTasNet/051_444_051c0101_1.9809_444o030u_-1.9809_pre2.wav?raw=true"></audio>

Conv-DPRNN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/DPRNN/051_444_051c0101_1.9809_444o030u_-1.9809_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/DPRNN/051_444_051c0101_1.9809_444o030u_-1.9809_pre2.wav?raw=true"></audio>

Our discrete Separation:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/051_444_051c0101_1.9809_444o030u_-1.9809_pre1.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/051_444_051c0101_1.9809_444o030u_-1.9809_pre2.wav?raw=true"></audio>

**(3) Sample3:** 

Mixture Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/Mix/22h_445_22ha010e_1.9643_445o030y_-1.9643.wav?raw=true">
</audio>

Conv-TasNet:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/ConvTasNet/22h_445_22ha010e_1.9643_445o030y_-1.9643_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/ConvTasNet/22h_445_22ha010e_1.9643_445o030y_-1.9643_pre2.wav?raw=true"></audio>

Conv-DPRNN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/DPRNN/22h_445_22ha010e_1.9643_445o030y_-1.9643_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/DPRNN/22h_445_22ha010e_1.9643_445o030y_-1.9643_pre2.wav?raw=true"></audio>

Our discrete Separation:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/22h_445_22ha010e_1.9643_445o030y_-1.9643_pre1.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/FM/22h_445_22ha010e_1.9643_445o030y_-1.9643_pre2.wav?raw=true"></audio>


### Male + Male

**(1) Sample1:** 

Mixture Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/Mix/22g_22h_22go010j_2.1114_22ho010c_-2.1114.wav?raw=true">
</audio>

Conv-TasNet:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/ConvTasNet/22g_22h_22go010j_2.1114_22ho010c_-2.1114_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/ConvTasNet/22g_22h_22go010j_2.1114_22ho010c_-2.1114_pre2.wav?raw=true"></audio>

Conv-DPRNN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/DPRNN/22g_22h_22go010j_2.1114_22ho010c_-2.1114_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/DPRNN/22g_22h_22go010j_2.1114_22ho010c_-2.1114_pre2.wav?raw=true"></audio>

Our discrete Separation:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/22g_22h_22go010j_2.1114_22ho010c_-2.1114_pre1.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/22g_22h_22go010j_2.1114_22ho010c_-2.1114_pre2.wav?raw=true"></audio>


**(2) Sample2:** 

Mixture Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/Mix/443_440_443o030y_1.7031_440o0308_-1.7031.wav?raw=true">
</audio>

Conv-TasNet:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/ConvTasNet/443_440_443o030y_1.7031_440o0308_-1.7031_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/ConvTasNet/443_440_443o030y_1.7031_440o0308_-1.7031_pre2.wav?raw=true"></audio>

Conv-DPRNN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/DPRNN/443_440_443o030y_1.7031_440o0308_-1.7031_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/DPRNN/443_440_443o030y_1.7031_440o0308_-1.7031_pre2.wav?raw=true"></audio>

Our discrete Separation:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/443_440_443o030y_1.7031_440o0308_-1.7031_pre1.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/443_440_443o030y_1.7031_440o0308_-1.7031_pre2.wav?raw=true"></audio>

**(3) Sample3:** 

Mixture Wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/Mix/443_22g_443c020w_1.0586_22go010u_-1.0586.wav?raw=true">
</audio>

Conv-TasNet:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/ConvTasNet/443_22g_443c020w_1.0586_22go010u_-1.0586_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/ConvTasNet/443_22g_443c020w_1.0586_22go010u_-1.0586_pre2.wav?raw=true"></audio>

Conv-DPRNN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/DPRNN/443_22g_443c020w_1.0586_22go010u_-1.0586_pre1.wav?raw=true"></audio>

<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/DPRNN/443_22g_443c020w_1.0586_22go010u_-1.0586_pre2.wav?raw=true"></audio>

Our discrete Separation:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/443_22g_443c020w_1.0586_22go010u_-1.0586_pre1.wav?raw=true"></audio>
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/shincling/discreteSeparation/blob/gh-pages/wavs/MM/443_22g_443c020w_1.0586_22go010u_-1.0586_pre2.wav?raw=true"></audio>

