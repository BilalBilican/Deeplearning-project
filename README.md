In this project, I build a 16 kHz speech accent classifier comparing two CNN pipelines: a RawCNN trained end-to-end on waveforms and a MelCNN trained on normalized log-mel 
spectrograms. Both use Adam with cross-entropy and identical data splits; I report accuracy, macro-F1, confusion matrices, and per-class recall. The mel-spectrogram model 
consistently outperforms the raw-audio baseline (~95.6% accuracy, 0.955 F1), and the error analysis surfaces accent-specific confusions and a small gender gap, suggesting 
class imbalance and room for stronger regularization/augmentation. The repo includes preprocessing scripts, model code, experiment configs, and notes on next steps 
(e.g., mixup, SpecAugment, or a raw+spectral fusion model).
 
