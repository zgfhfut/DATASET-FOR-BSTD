# DATASET-FOR-BSTD
Dataset for blind speech tampering detection (BSTD)

The careful configurations for both training and testing sets, incorporating MSFs and their corresponding GTMs. Note that each sample contains a set of MSFs and the corresponding GTM.

For DET-net training on Chinese speech data, we utilized 5,000 authentic samples and 20,000 tampered samples (5,000 per manipulation type), with 800 authentic and 3,200 tampered samples (800 per type) reserved for evaluation. For English speech data, the training set consisted of 4,500 authentic and 18,000 tampered samples (4,500 per type), while the evaluation set contained 800 authentic and 3,200 tampered samples (800 per type). Note that for testing purposes, we constructed a balanced testing set comprising 800 authentic speech samples and 800 manipulated audio samples of a specific tampering type, which were then processed through the network for evaluation.

For CLF-net training, we employed identical sample distributions for both Chinese and English speech data: 3,000 authentic and 12,000 tampered samples (3,000 per manipulation type) for training, with 1,000 authentic and 4,000 tampered samples (1,000 per type) allocated for evaluation. Notice that each sample is labeled with an integer (0-4) representing its category: non-tampering, copy-move forgery, deletion, homologous splicing, or heterologous splicing, respectively. In contrast to the testing approach used in DET-net, CLF-net is evaluated with a batch of 5,000 samples (1,000 authentic and 4,000 tampered) processed simultaneously.
