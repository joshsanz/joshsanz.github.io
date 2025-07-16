# My Research

My work explores key challenges in applying machine learning to wireless communication and sensing: learning communication protocols autonomously, automatic sensor calibration using environmental signals, and generating synthetic datasets for data-scarce domains.
The first portion explores interactive supervision for learning wireless PHY communication, where two independent agents develop a shared communication protocol without prior coordination.
The two agents are able to adapt by providing feedback in the form of echoing the other's message back, producing the minimal Echo Protocol for learning to communicate.
By introducing various levels of information sharing, the difficulty of the learning problem can be adjusted to balance prior coordination requirements and learning speed.
Experimental results show that even with limited information sharing, agents can achieve reliable communication, with applications in decentralized and adaptive wireless networks.
The work also investigates whether agents with different model architectures — so-called “alien agents” — can still learn to communicate effectively. Empirically, only the speed of learning (controlled by, e.g., the learning rate hyperparameter) matters, with faster learners being bottlenecked by slower ones.

The second portion focuses on environmental supervision for automatic sensing and calibration in distributed wireless networks.
The work introduces the use of signals of opportunity, such as ADS-B transmissions from aircraft and LEO satellite signals, to assess and calibrate radio spectrum sensors without requiring explicit cooperation from transmitters.
This approach enables automatic evaluation of sensor location, field of view, and indoor-outdoor placement among other possibilities.
This kind of automatic metadata extraction can mitigate challenges in crowd-sourced spectrum monitoring and large distributed networks, where sensor reliability and the trustworthiness of the sensor operator vary greatly.
The work also has regulatory implications due to discrepancies between how humans perceive 'indoorness' versus how radio propagation interacts with built structures.

The final portion tackles the issue of data scarcity by exploring the use of generative models to create synthetic datasets for wireless and biomedical signals.
Instead of relying on scarce real-world datasets, the study adapts image-based diffusion models to generate synthetic spectrograms of EEG signals, assessing their statistical similarity and utility for downstream classification tasks.
The findings highlight the need for careful validation of synthetic data, as distributional similarity does not always guarantee effective model training.
Together, my research contributes to advancing machine learning applications in wireless communication, spectrum sensing, and synthetic data generation, addressing critical bottlenecks in real-world deployment of adaptive "cognitive radio" systems.

## Publications

A. Sahai, **J. Sanz**, V. Subramanian, C. Tran, and K. Vodrahalli. 2019. Learning to Communicate with Limited Co-design. In _2019 57th Annual Allerton Conference on Communication, Control, and Computing (Allerton)_. IEEE Press, 184–191. doi: [10.1109/ALLERTON.2019.8919749](https://doi.org/10.1109/ALLERTON.2019.8919749).

A. Sahai, **J. Sanz**, V. Subramanian, C. Tran and K. Vodrahalli, "Blind Interactive Learning of Modulation Schemes: Multi-Agent Cooperation Without Co-Design," in _IEEE Access_, vol. 8, pp. 63790-63820, 2020, doi: [10.1109/ACCESS.2020.2984218](https://doi.org/10.1109/ACCESS.2020.2984218).

A. Abedi, **J. Sanz**, and A. Sahai, “Automatic Calibration in Crowd-Sourced Network of Spectrum Sensors,” in _Proceedings of the 22nd ACM Workshop on Hot Topics in Networks, ser. HotNets ’23_, Cambridge, MA, USA: Association for Computing Machinery, 2023, pp. 157–164. doi: [10.1145/3626111.3628187](https://doi.org/10.1145/3626111.3628187).

**J. Sanz**, A. Abedi, and A. Sahai, “Automatic Indoor-Outdoor Detection Using Signals of Opportunity,” in _2024 IEEE International Symposium on Dynamic Spectrum Access Networks (DySPAN)_, May 2024. doi: [10.1109/DySPAN60163.2024.10632851](https://doi.org/10.1109/DySPAN60163.2024.10632851).

A. Abedi, **J. Sanz**, and A. Sahai, “Using Signals of Opportunity to Establish Trust in Distributed Spectrum Monitoring Systems,” in _2024 IEEE International Symposium on Dynamic Spectrum Access Networks (DySPAN)_, 2024, pp. 33–38. doi: [10.1109/DySPAN60163.2024.10632745](https://doi.org/10.1109/DySPAN60163.2024.10632745).

A. Abedi, **J. Sanz**, M. Zheleva, and A. Sahai. 2024. From Foe to Friend: The Surprising Turn of Mega Constellations in Radio Astronomy. In _Proceedings of the 23rd ACM Workshop on Hot Topics in Networks (HotNets '24)_. Association for Computing Machinery, New York, NY, USA, 10–16. doi: [10.1145/3696348.3696863](https://doi.org/10.1145/3696348.3696863).

**J. Sanz**, “Lightly Supervised Machine Learning for Wireless Signals,” Ph.D. Thesis, EECS Department, University of California, Berkeley, 2024. Available [Online](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2024/EECS-2024-227.html).