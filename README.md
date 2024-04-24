# Conﬁdence Guided Semi-supervised Cross-Modality Person Re-Identiﬁcation
we propose a Conﬁdence Guided Semi-supervised Feature Learning (CGSFL) method for cross-modality person re-identiﬁcation, which can effectively exploit the information contained in unlabeled data with the help of a small amount of labeled data. Specially, the CGSFL framework consists of two key modules, including conﬁdence guided cross-modality pseudo label
generation module and semi-supervised cross-modality discriminant feature learning module. The former calculates the conﬁdence of cross-modality matching and clustering, utilizing them to enhance the reliability of generated cross-modality pseudo labels. The latter designs dynamic and static memory banks as well as a nearest neighbor class-based sampler to eﬀectively
exploit discriminant information present in labeled and pseudo-labeled data, thereby ensuring the discriminative capability of the learned model.

# Framework
fig1

# Requirement
Dependency packages that the environment may require: [requirements.txt](./requirements.txt)

# Dataset processing
Put SYSU-MM01 and RegDB dataset into data/sysu and data/regdb, run prepare\_sysu.py and prepare\_regdb.py to prepare the training data (convert to market1501 format).

# Train 
1. sh run\_train\_regdb.sh for RegDB
2. sh run\_train\_sysu.sh for SYSU-MM01

# Test 
1. sh run\_test\_regdb.sh for RegDB
2. sh run\_test\_sysu.sh for SYSU-MM01
