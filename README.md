# Privacy Enhancing Technology (PET)
Privacy-enhancing technologies (PET) are technologies that embody fundamental data protection principles by minimizing personal data use, maximizing data security, and empowering individuals. PETs allow online users to protect the privacy of their personally identifiable information (PII) provided to and handled by services or applications. PETs use techniques to minimize possession of personal data without losing the functionality of an information system.[1] Generally speaking, PETs can be categorized as hard and soft privacy technologies.
[Reference](https://en.wikipedia.org/wiki/Privacy-enhancing_technologies)

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

# NIST's Privacy Engineering Program (PEP)
Privacy engineering is integral to establishing trustworthiness in information systems that support the growth of the digital economy and improve individual quality of life. NIST research in information technology–including cybersecurity, cloud computing, big data, the Smart Grid and other cyber-physical systems–aims to improve the products and services that bring great advancements to U.S. national and economic security and quality of life. Much of this research pertains to the trustworthiness of these information technologies and the systems in which they are incorporated.

Given concerns about how information technologies may affect privacy at individual and societal levels, the PEP supports the development of trustworthy information systems by applying measurement science and system engineering principles to the creation of frameworks, risk models, guidance, tools, and standards that protect privacy and, by extension, civil liberties. [Reference](https://www.nist.gov/itl/applied-cybersecurity/privacy-engineering/about)

NIST Privacy Engineering [Reference](https://www.nist.gov/itl/applied-cybersecurity/privacy-engineering/about)
NIST Privacy Framework [Reference](https://www.nist.gov/system/files/documents/2020/01/16/NIST%20Privacy%20Framework_V1.0.pdf)
NIST Internal Report (NISTIR) 8062: An Introduction to Privacy Engineering and Risk Management in Federal Systems [Reference](https://doi.org/10.6028/NIST.IR.8062)
NIST Privacy Risk Assessment Methodology (PRAM) [Reference](https://www.nist.gov/document/nist-pram-feb2019zip)

# Privacy Engineering Collaboration Space
The NIST Privacy Engineering Collaboration Space is an online venue open to the public where practitioners can discover, share, discuss, and improve upon open source tools, solutions, and processes that support privacy engineering and risk management.
[Reference](https://github.com/usnistgov/PrivacyEngCollabSpace)

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


