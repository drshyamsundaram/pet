# Privacy Enhancing Technology (PET)
Privacy-enhancing technologies (PET) are technologies that embody fundamental data protection principles by minimizing personal data use, maximizing data security, and empowering individuals. PETs allow online users to protect the privacy of their personally identifiable information (PII) provided to and handled by services or applications. PETs use techniques to minimize possession of personal data without losing the functionality of an information system.[1] Generally speaking, PETs can be categorized as hard and soft privacy technologies.
[Reference](https://en.wikipedia.org/wiki/Privacy-enhancing_technologies)

# Anonymization methods[Reference](https://github.com/Nuclearstar/K-Anonymity)
Anonymization method aims at making the individual record be indistinguishable among a group record by using techniques of generalization and suppression.
The rapid growth of database, networking and computing technologies, a large amount of personal data can be integrated and analyzed digitally, leading to an increased use of data mining tools to infer trends and patterns.
This has been raised universal concerns about protecting the privacy of individuals.

## K-Anonymity [Reference](https://en.wikipedia.org/wiki/K-anonymity)[Reference](https://github.com/Nuclearstar/K-Anonymity)

k-anonymity is a property possessed by certain anonymized data. The concept of k-anonymity was first introduced by Latanya Sweeney and Pierangela Samarati in a paper published in 1998[1] as an attempt to solve the problem: "Given person-specific field-structured data, produce a release of the data with scientific guarantees that the individuals who are the subjects of the data cannot be re-identified while the data remain practically useful. A release of data is said to have the k-anonymity property if the information for each person contained in the release cannot be distinguished from at least {k-1} individuals whose information also appear in the release.

Turning a dataset into a k-anonymous (and possibly l-diverse or t-close) dataset is a complex problem, and finding the optimal partition into k-anonymous groups is an NP-hard problem. Fortunately, several practical algorithms exists that often produce "good enough" results by employing greedy search techniques.
In this tutorial we will explore the so-called "Mondrian" algorithm, which uses a greedy search algorithm to partition the original data into smaller and smaller groups (if we plot the resulting partition boundaries in 2D they resemble the pictures by Piet Mondrian, hence the name).
The algorithm assumes that we have converted all attributes into numerical or categorical values and that we are able to measure the “span” of a given attribute Xi.

## L-diversity[Reference](https://github.com/Nuclearstar/K-Anonymity)
l-diversity ensures that each k-anonymous group contains at least l different values of the sensitive attribute.
Therefore, even if an adversary can identify the group of a person he/she still would not be able to find out the value of that person's sensitive attribute with certainty.
Problem that might happen in k-anonymity is that all people in a k-anonymous group possess the same value of the sensitive attribute. An adversary who knows that a person is in that k-anonymous group can then still learn the value of the sensitive attribute of that person with absolute certainty. This problem can be fixed by using l-diversity.

## T-closeness[Reference](https://github.com/Nuclearstar/K-Anonymity)
t-closeness is a further refinement of l-diversity group based anonymization that is used to preserve privacy in data sets by reducing the granularity of a data representation.
This reduction is a trade off that results in some loss of effectiveness of data management or mining algorithms in order to gain some privacy.
The t-closeness model extends the l-diversity model by treating the values of an attribute distinctly by taking into account the distribution of data values for that attribute.
t-closeness demands that the statistical distribution of the sensitive attribute values in each k-anonymous group is "close" to the overall distribution of that attribute in the entire dataset.

# What is Differential Privacy
Differential privacy (DP) is a system for publicly sharing information about a dataset by describing the patterns of groups within the dataset while withholding information about individuals in the dataset. The idea behind differential privacy is that if the effect of making an arbitrary single substitution in the database is small enough, the query result cannot be used to infer much about any single individual, and therefore provides privacy. Another way to describe differential privacy is as a constraint on the algorithms used to publish aggregate information about a statistical database which limits the disclosure of private information of records whose information is in the database. For example, differentially private algorithms are used by some government agencies to publish demographic information or other statistical aggregates while ensuring confidentiality of survey responses, and by companies to collect information about user behavior while controlling what is visible even to internal analysts.

Roughly, an algorithm is differentially private if an observer seeing its output cannot tell if a particular individual's information was used in the computation. Differential privacy is often discussed in the context of identifying individuals whose information may be in a database. Although it does not directly refer to identification and reidentification attacks, differentially private algorithms probably resist such attacks.
[Reference](https://en.wikipedia.org/wiki/Differential_privacy)

Differential privacy was developed by cryptographers and thus is often associated with cryptography, and draws much of its language from cryptography.

# What is gradient descent
Gradient descent is a first-order iterative optimization algorithm for finding a local minimum of a differentiable function. The idea is to take repeated steps in the opposite direction of the gradient (or approximate gradient) of the function at the current point, because this is the direction of steepest descent. Conversely, stepping in the direction of the gradient will lead to a local maximum of that function; the procedure is then known as gradient ascent.
[Reference](https://en.wikipedia.org/wiki/Gradient_descent)

# Implement Differential Privacy with TensorFlow Privacy
Differential privacy (DP) is a framework for measuring the privacy guarantees provided by an algorithm. Through the lens of differential privacy, you can design machine learning algorithms that responsibly train models on private data. Learning with differential privacy provides measurable guarantees of privacy, helping to mitigate the risk of exposing sensitive training data in machine learning. Intuitively, a model trained with differential privacy should not be affected by any single training example, or small set of training examples, in its data set. This helps mitigate the risk of exposing sensitive training data in ML.
TensorFlow Privacy provides code that wraps an existing TensorFlow optimizer to create a variant that implements DP-SGD.[Reference](https://github.com/tensorflow/privacy/tree/master/tutorials/walkthrough) [Reference](https://github.com/tensorflow/privacy/tree/master/tutorials/walkthrough)

# Differential Privacy autoencoder-based generative model
## Differentially private autoencoder-based generative model (DP-AuGM)
This approach is to share models, where we encode the information of the data into a machine learning model for learning data representations and then share the machine learning model instead.

## Differentially private variational autoencoder-based generative model (DP-VaeGM)
This approach is to share data, where we use the shared data for training a generative model which learns the distribution of the data, and then the generative model is used to generate a new dataset for usage and the new dataset can be
shared further.

For futher detailed reading , please peruse the article, 'Differentially Private Data Sharing | Sharing Models versus Sharing Data' [Reference](https://chenqingrong.github.io/files/dpgm.pdf)

# Usecases
## US Census
Explains the Census Bureau’s decision to modernize the methods we use to protect respondent confidentiality. The adoption of DF and concepts of disclosure avoidance and differential privacy and discuss their implications for census data users. [Reference](https://chenqingrong.github.io/files/dpgm.pdf)

The use of differential privacy for census data and its impact on redistricting: The case of the 2020 U.S. Census [Reference](https://www.science.org/doi/10.1126/sciadv.abk3283)

# NIST's Privacy Engineering Program (PEP)
Privacy engineering is integral to establishing trustworthiness in information systems that support the growth of the digital economy and improve individual quality of life. NIST research in information technology–including cybersecurity, cloud computing, big data, the Smart Grid and other cyber-physical systems–aims to improve the products and services that bring great advancements to U.S. national and economic security and quality of life. Much of this research pertains to the trustworthiness of these information technologies and the systems in which they are incorporated.

Given concerns about how information technologies may affect privacy at individual and societal levels, the PEP supports the development of trustworthy information systems by applying measurement science and system engineering principles to the creation of frameworks, risk models, guidance, tools, and standards that protect privacy and, by extension, civil liberties. [Reference](https://www.census.gov/data/academy/webinars/2021/disclosure-avoidance-series/differential-privacy-101.html)

NIST Privacy Engineering [Reference](https://www.nist.gov/itl/applied-cybersecurity/privacy-engineering/about)
NIST Privacy Framework [Reference](https://www.nist.gov/system/files/documents/2020/01/16/NIST%20Privacy%20Framework_V1.0.pdf)
NIST Internal Report (NISTIR) 8062: An Introduction to Privacy Engineering and Risk Management in Federal Systems [Reference](https://doi.org/10.6028/NIST.IR.8062)
NIST Privacy Risk Assessment Methodology (PRAM) [Reference](https://www.nist.gov/document/nist-pram-feb2019zip)

# Privacy Engineering Collaboration Space
The NIST Privacy Engineering Collaboration Space is an online venue open to the public where practitioners can discover, share, discuss, and improve upon open source tools, solutions, and processes that support privacy engineering and risk management.
[Reference](https://github.com/usnistgov/PrivacyEngCollabSpace)

# References - General 
1. NIST Privacy Engineering [Reference](https://www.nist.gov/itl/applied-cybersecurity/privacy-engineering/about)
2. NIST Privacy Framework [Reference](https://www.nist.gov/system/files/documents/2020/01/16/NIST%20Privacy%20Framework_V1.0.pdf)
3. NIST Internal Report (NISTIR) 8062: An Introduction to Privacy Engineering and Risk Management in Federal Systems [Reference](https://doi.org/10.6028/NIST.IR.8062)
4. NIST Privacy Risk Assessment Methodology (PRAM) [Reference](https://www.nist.gov/document/nist-pram-feb2019zip)
5. Privacy Engineering Collaboration Space [Reference](https://github.com/usnistgov/PrivacyEngCollabSpace)
6. Model Open Data Benefit Risk Analysis [Reference](https://fpf.org/blog/fpf-publishes-model-open-data-benefit-risk-analysis/) [Reference](https://fpf.org/wp-content/uploads/2018/01/Model-Benefit-Risk-Analysis.pdf)

# References - Differential Privacy
1. Gradient descent [Reference](https://en.wikipedia.org/wiki/Gradient_descent)
2. Differential Privacy Series Part 1 | DP-SGD Algorithm Explained [Reference](https://medium.com/pytorch/differential-privacy-series-part-1-dp-sgd-algorithm-explained-12512c3959a3)
3. Implement Differential Privacy with TensorFlow Privacy| DP-SGD Algorithm Explained [Reference](https://www.tensorflow.org/responsible_ai/privacy/tutorials/classification_privacy)
4. Machine learning with differential privacy in tensorflow [Reference](http://www.cleverhans.io/privacy/2019/03/26/machine-learning-with-differential-privacy-in-tensorflow.html)
5. Differential Privacy in Deep Learning - A practical guide on how Differential Privacy is integrated into Deep Learning architectures for image classification [Reference](https://towardsdatascience.com/differential-privacy-in-deep-learning-cf9cc3591d28)
6. DIFFERENTIALLY PRIVATE DEEP LEARNING IN 20 LINES OF CODE: HOW TO USE THE PYTORCH OPACUS LIBRARY [Reference](https://blog.openmined.org/differentially-private-deep-learning-using-opacus-in-20-lines-of-code/)
7. How to deploy machine learning with differential privacy, Nicolas Papernot and Abhradeep Guha Thakurta [Reference](https://en.wikipedia.org/wiki/Gradient_descent](https://www.nist.gov/blogs/cybersecurity-insights/how-deploy-machine-learning-differential-privacy)
8. A Differentially Private Data Analytics API at Scale,Ryan Rogers, LinkedIn [Reference](https://www.usenix.org/conference/pepr20/presentation/rogers)
9. Google DP Library [Reference](https://github.com/google/differential-privacy)
10. Boyd, Danah and Sarathy, Jayshree, Differential Perspectives: Epistemic Disconnects Surrounding the US Census Bureau’s Use of Differential Privacy (March 15, 2022). Harvard Data Science Review (Forthcoming) , [Reference](https://ssrn.com/abstract=4077426)
11. Platform-for-differential-privacy [Reference](https://www.microsoft.com/en-us/research/publication/platform-for-differential-privacy/)
12. new-differential-privacy-platform-microsoft-harvard-opendp [Reference](https://cloudblogs.microsoft.com/opensource/2020/05/19/new-differential-privacy-platform-microsoft-harvard-opendp/)
13. Opendp [Reference](https://github.com/opendp)
14. How do deploy machine learning with DP (NIST Blog) [Reference](https://www.nist.gov/blogs/cybersecurity-insights/how-deploy-machine-learning-differential-privacy)

# References - k-anonimity
1. K-anonymity [Reference](https://en.wikipedia.org/wiki/K-anonymity)
2. K-anonymity: A MODEL FOR PROTECTING PRIVACY LATANYA SWEENEY [Reference](https://epic.org/wp-content/uploads/privacy/reidentification/Sweeney_Article.pdf)
3. K-anonymity Implementation References (Nuclearstar github) |  [Reference](https://github.com/Nuclearstar/K-Anonymity)
4. An intoduction (privitar) [Reference](https://www.privitar.com/blog/k-anonymity-an-introduction/)
5. K-anonymity Slides [Reference](https://www.cs.cmu.edu/~jblocki/Slides/K-Anonymity.pdf)
6. K-anonymity Glossary (NIST) [Reference](https://csrc.nist.gov/glossary/term/k_anonymity)
7. K-anonymity Samarati_Sweeney Paper [Reference](https://epic.org/wp-content/uploads/privacy/reidentification/Samarati_Sweeney_paper.pdf)

# ARX Tool
ARX is a comprehensive open source software for anonymizing sensitive personal data. It has been designed from the ground up to provide high scalability, ease of use and a tight integration of the many different aspects relevant to data anonymization. Its highlights include:
Utility-focused anonymization using different statistical models
Syntactic privacy models, such as k-anonymity, ℓ-diversity, t-closeness and δ-presence
Semantic privacy models, such as (ɛ, δ)-differential privacy
Methods for optimizing the profitability of data publishing based on monetary cost-benefit analyses
Data transformation with generalization, suppression, microaggregation and top/bottom coding as well as global and local recoding
Methods for analyzing data utility
Methods for analyzing re-identification risks
Tool download : [Reference](https://arx.deidentifier.org/downloads/)
Configuration : [Reference](https://arx.deidentifier.org/anonymization-tool/configuration/)
Github : [Reference](https://github.com/arx-deidentifier/arx)

# Gretal.ai [Reference](https://gretel.ai/)
Gretel.ai automates privacy engineering, enabling companies to reduce the time to access sensitive data by up to 10x and backed by mathematical privacy guarantees
Tool download : [Reference](https://console.gretel.cloud/login)
Docs : [Reference](https://docs.gretel.ai/)
Github : [Reference](https://github.com/gretelai)
Article : [Reference](https://medium.com/gretel-ai/using-generative-differentially-private-models-to-build-privacy-enhancing-synthetic-datasets-c0633856184)
