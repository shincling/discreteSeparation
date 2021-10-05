## Discretization and Re-synthesis: an alternative method to solve the Cocktail Party Problem

### Abstract
Neural network based models have significantly improved the performance of speech separation with the input waveform from scenarios like the cocktail party. Prominent methods (e.g., frequency-domain and time-domain speech separation) usually build regression model to recover the ground-truth speech as much as possible, with the masking-based design and the signal-level loss criterion (e.g., MSE or SI-SNR). We propose here that the synthesis-based approach can also perform well towards this problem, with great flexibility and potential.  Specifically, we propose a novel speech separation/enhancement model based on the recognition of discrete symbols, converting the paradigm of the speech separation/enhancement related tasks from regression problem to classification task. By utilizing the synthesis model with the input of discrete symbols, after the prediction of discrete symbol sequence, each target speech could be re-synthesized. The experimental evaluation with the WSJ0-2mix and VCTK-noisy corpus in various settings shows that the proposed method could steadily synthesize the separated speech of good listening quality, nearly without any interference, which is difficult to avoid in regression based methods. In addition, with quite little loss of listening quality, the speaker conversion of enhanced/separated speech could be easily realized through our method.

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/shincling/discreteSparation/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
