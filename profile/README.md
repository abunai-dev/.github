<p align="center"> 
	<h3 align="center"><img alt="ABUNAI" src="abunai-art.png"><br>
    ABUNAI</h3>
</p>
<p>&nbsp;</p>

## Architecture-Based and Uncertainty-Aware Confidentiality Analysis

[![xDECAF analysis framework](https://img.shields.io/badge/xDECAF%20analysis%20framework-v4.0.0-orange?style=flat-square&logo=eclipse&logoColor=white)](https://dataflowanalysis.org)
[![Dissertation](https://img.shields.io/badge/Dissertation-Available-green?style=flat-square&logo=GitBook&logoColor=white)](https://doi.org/10.5445/IR/1000178700)
[![Overview Slides](https://img.shields.io/badge/Overview%20Slides-Available-green?style=flat-square&logo=Slides&logoColor=white)](https://sebastianhahner.de/talks/2024/DoctoralDefenseSebastianHahner_2024_ArchitectureBasedAndUncertaintyAwareConfidentialityAnalysis.pdf)
[![Uncertainty Catalog](https://img.shields.io/badge/Uncertainty%20Catalog-Available-green?style=flat-square&logo=github)](https://arc3n.abunai.dev)

**ABUNAI** is a research approach for confidentiality analysis under uncertainty.
It comprises a classification of uncertainty regarding confidentiality, a catalog of uncertainty sources, an uncertainty impact analysis that propagates uncertainty to predict its impact on the system's confidentiality, and uncertainty-aware confidentiality analyses that identify violations of confidentiality requirements with respect to uncertainty.
The central idea is to represent classified uncertainty as first-class entity in confidentiality analysis:
<p>&nbsp;</p>

![Overview](overview-light.png#gh-light-mode-only)
![Overview](overview-dark.png#gh-dark-mode-only)

The project's name is inspired by the Japanese word **あぶない (abunai)** which translates to dangerous, risky, or uncertain.
The research project was started as the dissertation project of [Dr.-Ing. Sebastian Hahner](https://sebastianhahner.de) at the DSiS group, Karlsruhe Institute of Technology (KIT).

For a comprehensive introduction and details on both the analysis and its evaluation, please see the published dissertation:

* S. Hahner, "Architecture-Based and Uncertainty-Aware Confidentiality Analysis", Karlsruhe Institute of Technology (KIT), Dissertation, 2024, doi: [10.5445/IR/1000178700](https://doi.org/10.5445/IR/1000178700).

More information can be found in these key publications:

* S. Hahner, et al., "ARC³N: A Collaborative Uncertainty Catalog to Address the Awareness Problem of Model-Based Confidentiality Analysis", MODELS-C, ACM/IEEE, 2024, doi: [10.1145/3652620.3688556](https://doi.org/10.1145/3652620.3688556).
* S. Hahner, et al., "A Classification of Software-Architectural Uncertainty Regarding Confidentiality", ICETE, Springer, 2023, doi:  [10.1007/978-3-031-36840-0_8](https://doi.org/10.1007/978-3-031-36840-0_8).
* S. Hahner, et al., "Architecture based Uncertainty Impact Analysis to Ensure Confidentiality", SEAMS, IEEE/ACM, 2023, doi: [10.1109/SEAMS59076.2023.00026](https://doi.org/10.1109/SEAMS59076.2023.00026).
* S. Hahner, et al., "Model-based Confidentiality Analysis under Uncertainty", ICSA-C, IEEE, 2023, doi: [10.1109/ICSA-C57050.2023.00062](https://doi.org/10.1109/ICSA-C57050.2023.00062).

## Procedure

The ABUNAI approach comprises four steps to handle the effect of uncertainty on architecture-based confidentiality analysis:

1. [**Identification and awareness**](https://github.com/abunai-dev/ARC3N): To include uncertainty sources in the analysis, they must be known first. Thus, raising awareness to recognize the presence of uncertainty in a system is the necessary first step.
2. [**Classification**](https://github.com/abunai-dev/ARC3N): To better understand the type of uncertainty sources and their properties, they can be classified. To that end, classifications and taxonomies provide the foundations for the documentation and the discussion of identified uncertainty.
3. [**Propagation**](https://github.com/abunai-dev/UncertaintyImpactAnalysis): To assess the impact of identified and classified uncertainty sources, they can be propagated through the architectural model. Estimating the potential impact early helps in making more precise statements and decisions.
4. [**Analysis**](https://github.com/abunai-dev/ABUNAI): To apply appropriate mitigation strategies, the effect of uncertainty on the software system's quality has to be analyzed. In our case, this means identifying confidentiality violations due to the identified, classified, and propagated uncertainty.

<p>&nbsp;</p>
![Procedure](procedure-light.png#gh-light-mode-only)
![Procedure](procedure-dark.png#gh-dark-mode-only)

For more information, please read *Chapter 4.1* in the [dissertation](https://doi.org/10.5445/IR/1000178700).


## Organization Structure

The repositories of this organization contain all relevant ABUNAI artifacts:

* [ARC³N](https://github.com/abunai-dev/ARC3N) contains a catalog of classified uncertainty sources, available [online](https://arc3n.abunai.dev/).
* [Uncertainty Impact Analysis](https://github.com/abunai-dev/UncertaintyImpactAnalysis) contains an analysis to predict the impact of uncertainty on confidentiality.
* [ABUNAI](https://github.com/abunai-dev/ABUNAI) contains the core analysis to identify confidentiality violations with respect to uncertainty.

Furthermore, we provide the scenarios used in the evaluation of the approach, see [here](https://doi.org/10.5445/IR/1000178700). This includes the [CoronaWarnApp](https://github.com/abunai-dev/EvaluationScenario-CoronaWarnApp), [OnlineShop](https://github.com/abunai-dev/EvaluationScenario-OnlineShop), [Jplag](https://github.com/abunai-dev/EvaluationScenario-JPlag), and [MobilityAsAService](https://github.com/abunai-dev/EvaluationScenario-MaaS) scenarios. Further examples can be found in the [xDECAF organization](https://github.com/DataFlowAnalysis/DataFlowAnalysis).
