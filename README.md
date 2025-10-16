🧠 Comprehensive Explanation of the Experiment
This experiment explores the use of self-supervised vision transformers (DINO) for extracting robust medical image representations. The objective is to assess whether pre-trained DINO encoders, originally trained on ImageNet, can effectively capture discriminative features from specialized domains such as chest X-rays or pneumonia scans.
The model processes grayscale medical images, converts them into RGB tensors, and generates feature embeddings that can be applied to classification, clustering, or anomaly detection tasks. The workflow includes data preprocessing, feature extraction, linear probing, and visualization through PCA.
This approach highlights how representation learning can replace expensive labeled data, enabling efficient transfer learning in medical imaging.

✏️ Objective
To demonstrate how self-supervised representations from DINO can generalize to unseen medical domains, providing a foundation for accurate downstream diagnostic models. The experiment aims to validate that DINO embeddings encode meaningful structural and semantic patterns even without retraining.

📘 Results

DINO embeddings achieved high separability between healthy and diseased samples using a simple linear probe.

Visualization via PCA showed clear cluster distinction, confirming feature richness and consistency.

Accuracy of the linear classifier exceeded baseline supervised CNNs trained from scratch.

The results suggest that self-supervised transformers can accelerate research in specialized imaging without large annotated datasets.

📓 Observations

DINO’s ViT-S/16 model provided stable feature embeddings despite limited dataset size.

Minimal preprocessing was required, proving the robustness of the learned representations.

Transfer learning from natural to medical imagery succeeded with excellent generalization capability.

Future work could integrate domain adaptation techniques or fine-tune specific layers for even higher medical diagnostic accuracy.
