# Gaussian Flow Bridges for audio domain transfer with unpaired data

Audio domain transfer is the process of modifying audio signals
to match characteristics of a different domain, while retaining the
original content. This paper investigates the potential of Gaussian
Flow Bridges, an emerging approach in generative modeling, for this
problem. The presented framework addresses the transport prob-
lem across different distributions of audio signals through the im-
plementation of a series of two deterministic probability flows. The
proposed framework facilitates manipulation of the target distribu-
tion properties through a continuous control variable, which defines
a certain aspect of the target domain. Notably, this approach does
not rely on paired examples for training. To address identified chal-
lenges on maintaining the speech content consistent, we recommend
a training strategy that incorporates chunk-based minibatch Optimal
Transport couplings of data samples and noise. Comparing our un-
supervised method with established baselines, we find competitive
performance in tasks of reverberation and distortion manipulation.
Despite encoutering limitations, the intriguing results obtained in
this study underscore potential for further exploration.

In this repository, we provide the sample code to train a Gaussian Flow Bridge (GFB) for controlling speech reverberation or clipping, presented in the paper ["Gaussian Flow Bridges for audio domain transfer with unpaired data"](https://) submitted to IEEE IWAENC 2024. 
We hope this sample code enables reproducibility of our proposed method and results and invites further work on the topic of audio domain transfer.
The samples folder includes some audio examples. 

## Paper
If you use this code in your research please cite the following [publication](https://):
```
@inproceedings{emoliner2024,
  title={Gaussian Flow Bridges for audio domain transfer with unpaired data},
  author={Moliner, Eloi and Braun, Sebastian and Gamper, Hannes},
  journal={arxiv},
  notes={Submitted to IEEE IWAENC 2024}
}
```

This paper can also be found on arXiv at [...](...).

-----
[LICENSE](https://github.com/microsoft/GFB-audio-control/blob/master/LICENSE)


[Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct)

-----

## Responsible AI Transparency Information 

An AI system includes not only the technology, but also the people who will use it, the people who will be affected by it, and the environment in which it is deployed. Creating a system that is fit for its intended purpose requires an understanding of how the technology works, its capabilities and limitations, and how to achieve the best performance. Microsoft has a broad effort to put our AI principles into practice. To find out more, see [Responsible AI principles from Microsoft](https://www.microsoft.com/en-us/ai/responsible-ai). 

### Use of this code 

The purpose of this sample code is to enable reproducibility of our method and results and to encourage future work on the topic. 

### Project data 

The sample folder contains a selection of audio samples illustrating the performance of the proposed model. The samples are taken from the publicly available [DAPS dataset](https://zenodo.org/records/4660670). 

### Fairness and Responsible AI testing 

At Microsoft, we strive to empower every person on the planet to do more. An essential part of this goal is working to create technologies and products that are fair and inclusive. Fairness is a multi-dimensional, sociotechnical topic and impacts many different aspects of our work.  

When systems are deployed, Responsible AI testing should be performed to ensure safe and fair operation for the specific use case. No Responsible AI testing has been done to evaluate this method including validating fair outcomes across different groups of people. Responsible AI testing should be done before using this code in any production scenario. 

> Note: The documentation included in this ReadMe file is for informational purposes only and is not intended to supersede the applicable license terms. 

## Contributing

This code has been created as part of a summer intern project by Eloi Moliner ( email ), Ph.D. Student, Aalto University, Finland

---

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Requirements

We recommend using the [Anaconda](https://docs.anaconda.com/anaconda/install/) distribution for python dependencies. The code should work will any recent version. In addition, the following packages are required:

- Pytorch (https://pytorch.org/) -> All recent versions should work. Tested on 1.8 and newers. 
- Click (`pip install click`) -> All recent versions should work. Tested on 6.5 and newers.
- Pyprind (`pip install PyPrind`) -> All versions should work. 

## How to use

### Step 0) Data Preparation: 

---

### Step 1) Train the Gaussian Diffusion Bridge model

-----

### Step 2) Run evaluation scripts

