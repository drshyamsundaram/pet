# Privacy Enhancing Technology (PET)
Privacy-enhancing technologies (PET) are technologies that embody fundamental data protection principles by minimizing personal data use, maximizing data security, and empowering individuals. PETs allow online users to protect the privacy of their personally identifiable information (PII) provided to and handled by services or applications. PETs use techniques to minimize possession of personal data without losing the functionality of an information system.[1] Generally speaking, PETs can be categorized as hard and soft privacy technologies.
[Reference](https://en.wikipedia.org/wiki/Privacy-enhancing_technologies)

# What is Differential Privacy
Differential privacy (DP) is a system for publicly sharing information about a dataset by describing the patterns of groups within the dataset while withholding information about individuals in the dataset. The idea behind differential privacy is that if the effect of making an arbitrary single substitution in the database is small enough, the query result cannot be used to infer much about any single individual, and therefore provides privacy. Another way to describe differential privacy is as a constraint on the algorithms used to publish aggregate information about a statistical database which limits the disclosure of private information of records whose information is in the database. For example, differentially private algorithms are used by some government agencies to publish demographic information or other statistical aggregates while ensuring confidentiality of survey responses, and by companies to collect information about user behavior while controlling what is visible even to internal analysts.

Roughly, an algorithm is differentially private if an observer seeing its output cannot tell if a particular individual's information was used in the computation. Differential privacy is often discussed in the context of identifying individuals whose information may be in a database. Although it does not directly refer to identification and reidentification attacks, differentially private algorithms probably resist such attacks.
[Reference](https://en.wikipedia.org/wiki/Differential_privacy)

Differential privacy was developed by cryptographers and thus is often associated with cryptography, and draws much of its language from cryptography.

# References - Differential Privacy
1. Differential Privacy Series Part 1 | DP-SGD Algorithm Explained [Reference](https://medium.com/pytorch/differential-privacy-series-part-1-dp-sgd-algorithm-explained-12512c3959a3)
2. Implement Differential Privacy with TensorFlow Privacy| DP-SGD Algorithm Explained [Reference](https://www.tensorflow.org/responsible_ai/privacy/tutorials/classification_privacy)
