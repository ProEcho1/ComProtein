# ComProtein
Proteins serve as the functional building blocks of life, facilitating critical tasks such as signaling, catalysis, and structural support in all living organisms. Designing proteins with targeted biological features or domains is of utmost importance. Traditional wet-lab experiments are time-consuming and resource-intensive, which makes deep learning (DL) methods ideal alternatives. However, existing DL methods predominantly focus on generating new proteins with the same biological domain as the training data, and overlook some scenarios where designers expect to combine proteins from different biological domains to create novel proteins with both features, which can show better fits for practical purpose. To fill this gap, in this paper, we present \textsc{ComProtein}, a novel framework further exploiting the potential of pre-trained protein large language models, which is the \textit{first} work aiming to generate innovative proteins with combinative biological features from two different domains. This process is performed by a cycle-consistent generative adversarial approach, leveraging insights from the latent space. It enables the transformation of protein representations from one biological domain to another, while preserving their intrinsic features. Additionally, we introduce new evaluative metrics, namely Shortest Target Neighbor Distance (STND), Mutual Root Mean Square Deviation (MRMSD) and Sequence Diversity (SD) on the evaluation of biological representations, protein structure and sequence quality, respectively to complement the existing measures. Our experimental results demonstrate that our proposed method performs better and has great potential in biological representations, structure similarity, homology relationships, and sequence quality.

It's our great hornor to get you attention to our work ComProtein. Pre-trained checkpoints and splited data will be available once acceptance and more details will be added soon.

# Model Architecture
![Model Architecture](images/model.pdf)

# Closely Related Generation
|  |  |  |  |
|---|---|---|---|
| ![alt text](images/C1.png "Domain A - A")   | ![alt text](images/C2.png "Domain A - B") | ![alt text](images/C3.png "Domain B - A")   | ![alt text](images/C4.png "Domain B - B") |
| (a) Domain A - A   | (b) Domain A - B | (c) Domain B - A   | (d) Domain B - B |
| ![alt text](images/C5.png "Generated - A")  | ![alt text](images/C6.png "Generated - B")  | ![alt text](images/C7.png "Generated - C") | ![alt text](images/C8.png "Generated - D") |
| (a) Generated - A   | (b) Generated - B | (c) Generated - C   | (d) Generated - D |

# Distantly Related Generation
|  |  |  |  |
|---|---|---|---|
| ![alt text](images/D1.png "Domain A - A")   | ![alt text](images/D2.png "Domain A - B") | ![alt text](images/D3.png "Domain B - A")   | ![alt text](images/D4.png "Domain B - B") |
| (a) Domain A - A   | (b) Domain A - B | (c) Domain B - A   | (d) Domain B - B |
| ![alt text](images/D5.png "Generated - A")  | ![alt text](images/D6.png "Generated - B")  | ![alt text](images/D7.png "Generated - C") | ![alt text](images/D8.png "Generated - D") |
| (a) Generated - A   | (b) Generated - B | (c) Generated - C   | (d) Generated - D |
