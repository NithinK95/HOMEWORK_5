# HOMEWORK_5
NITHIN AARON KOMMIREDDY      700752900

README: AI Tasks and Solutions
This document covers the solutions for six different programming tasks related to AI, including GAN implementation, data poisoning simulation, and more.

Table of Contents
GAN Architecture

Ethics and AI Harm

Programming Task (Basic GAN Implementation)

Programming Task (Data Poisoning Simulation)

Legal and Ethical Implications of GenAI

Bias & Fairness Tools

1. GAN Architecture
Adversarial Process in GAN Training
The adversarial process involves two neural networks: the Generator and the Discriminator. The Generator tries to create realistic data (e.g., images) to deceive the Discriminator, which aims to distinguish between real and fake data. Over time, through this competition, both networks improve their performance.

Generator's Goal: To generate fake data that closely resembles real data.

Discriminator's Goal: To differentiate between real data and data generated by the Generator.

Through alternating updates and backpropagation, both networks improve over time, with the Generator creating increasingly realistic data and the Discriminator becoming better at distinguishing fake from real data.

GAN Architecture Diagram
A diagram has been included that illustrates the architecture of a basic GAN, showing the data flow between the Generator, Discriminator, and the real data.

2. Ethics and AI Harm
Topic: Misinformation in Generative AI
A hypothetical example of how misinformation can occur in generative AI is when models like GPT-3 generate false information due to biases or lack of real-world context. For instance, a model trained on biased or incorrect sources might generate unreliable health advice.

Mitigation Strategies:

Use curated and verified data sources for training.

Implement fact-checking mechanisms within the model to flag potentially harmful or incorrect content.

3. Programming Task (Basic GAN Implementation)
Task: Basic GAN Implementation for MNIST
This task involves implementing a simple GAN in PyTorch to generate handwritten digits from the MNIST dataset.

Generator Architecture: A simple fully connected neural network that takes random noise as input and outputs a 28x28 image of a handwritten digit.

Discriminator Architecture: A neural network that classifies input images as real or fake.

The GAN is trained for 101 epochs, and sample images are shown at epochs 0, 50, and 100. Losses of the generator and discriminator are also plotted over time.

4. Programming Task (Data Poisoning Simulation)
Task: Data Poisoning Attack on Sentiment Classifier
This task simulates a data poisoning attack on a sentiment classifier. In this case, we poisoned the dataset by flipping the sentiment labels for reviews that mention a specific entity (e.g., "UC Berkeley").

Before Poisoning: The classifier is trained on a clean dataset and performs well with good accuracy and confusion matrix metrics.

After Poisoning: The classifier’s performance decreases significantly as the poisoned labels introduce noise, making the model misclassify certain reviews.

Result Graphs
The simulation shows a clear drop in accuracy and an increase in misclassifications after the poisoning attack.

5. Legal and Ethical Implications of GenAI
Concerns About AI-Generated Content
Generative AI models raise legal and ethical concerns such as:

Memorizing Private Data: Models like GPT-2 may inadvertently memorize private data, such as personal names or addresses, leading to privacy violations.

Generating Copyrighted Material: AI models can generate content that closely resembles copyrighted material, leading to intellectual property issues.

Should Generative AI be restricted from certain data during training?
Yes. Restricting models from training on sensitive or copyrighted data helps prevent ethical and legal issues. Without restrictions, models may generate outputs that infringe on privacy or intellectual property rights.

6. Bias & Fairness Tools
Bias Metric: False Negative Rate Parity
This metric measures whether the false negative rate (FNR) is equal across different demographic groups.

Importance: It ensures that no group is unfairly impacted by higher false negatives (e.g., false positives may not be as harmful).

Failure Scenario: A model might fail this metric if it has a higher FNR for one demographic group compared to others, such as minorities being misclassified more often.
