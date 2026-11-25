# Character and Digit recognition CNN with 90%+ accuracy trained and tested on the EMNIST ByMerge Dataset

## How to run
- Run the command (installs required packages):
```bash
pip install -r requirements.txt
```
- The EMNIST Dataset downloads automatically when the notebook is run.

## Architecture
- 3-layer CNN with 2 fully-connected layers.
- PReLU layers reduce dying neurons compared to ReLU.
- BatchNorm2D layers stabilise the gradients.
- Used CrossEntropy Loss
- Used SGD Optimizer with an initial learning rate of 0.01 and momentum of 0.9.
- Used a ReduceLROnPlateau scheduler to reduce the learning rate when training loss plateaus.

## Results (Trained for ~20 epochs (may have been stopped slightly earlier))
- Accuracy: 90.5521693904043%
- Loss: 0.27659484301949594
