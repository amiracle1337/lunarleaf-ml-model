# LunarLeaf: Plant Health Detection via CNNs

LunarLeaf employs Convolutional Neural Networks (CNNs) to discern the health status of tomato plants using leaf images.

![LG UltraFine](https://user-images.githubusercontent.com/122039464/273696199-9e123fa9-82ae-45c3-8776-0fbfef79cab6.jpg)

## Model Architecture and Design Process

1. **Data Pre-processing**: Ensuring the quality of the dataset was trivial to making the model work. Pre-processing steps were implemented to guarantee clean and robust data for training.

2. **Model Exploration**: I delved deep into various model architectures to identify the best fit:
   - Leveraged the renowned **VGG16** architecture, which excelled in training and validation but demonstrated overfitting on test data.
   - Experimented with simpler models based on advice regarding the potential of complex models overfitting. These models performed adequately on training and validation, but their test performance was lacking.
   - Engaged in extensive iterative testing with over 20 different architectural variations, altering layer depths, filter counts, units in dense layers, and more.
   - Adjusted learning rates to optimize performance.

3. **Optimal Architecture**: The model's peak performance was achieved with layers deepening progressively and filters doubling in each successive layer. Such design allowed the model to capture intricate details and nuances in the tomato leaves, resulting in superior generalization. Tweaks beyond this architecture, including modifying layer counts or adjusting dense units, compromised the model's accuracy.

## Additional Notes

- This venture into machine learning and Python coding marks my debut.
- The inception of **LunarLeaf** was born from a practical need: in collaboration with physicist Twana Cheragwandi, we constructed an indoor aeroponic farm to cultivate vegetables. To streamline our workflow, we envisioned an automated system where a robot would capture daily images of the plants, which **LunarLeaf** would then analyze, ensuring the plants' optimal health.

![Screenshot 2023-10-09 at 23 19 28](https://github.com/amiracle1337/lunarleaf/assets/122039464/769e955e-e046-437c-b6a8-a71edae66a84)
