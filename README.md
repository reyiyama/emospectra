# Emotion Spectrum Visualization Tool

## Repository Name: **EmoSpectra**

### Introduction
Welcome to **EmoSpectra**, a sentiment analysis project that goes beyond traditional emotional models to create a comprehensive, culturally-inclusive, and visually intuitive representation of human emotions. By integrating emotions from a wide variety of cultures, **EmoSpectra** leverages data-driven techniques, such as t-Distributed Stochastic Neighbor Embedding (t-SNE) and clustering with k-means, to map the full emotional spectrum in an interactive 3D space. This visualization captures the complexity of human emotions in a way that encourages empathy and deeper understanding of different cultural experiences.

This project aims to empower stakeholders—such as NGOs, research institutes, and mental health professionals—by providing an expanded emotional model that incorporates lesser-known cultural emotions. Our work is grounded in ethical, transparent, and accountable practices, making it a useful tool for sentiment analysis, activism, and various applications that demand an in-depth understanding of human emotions.

### Inspiration & Brainstorming Journey
The development of this project was inspired by the limitations we found in popular sentiment analysis tools, which often rely on binary reactions (e.g., likes/dislikes) or only consider a narrow set of emotions. During our brainstorming sessions, our group researched Plutchik's Wheel of Emotions, which identifies eight basic emotions, and quickly realized that the model falls short of capturing the complexity of emotions experienced by different communities, particularly indigenous and marginalized cultures. **EmoSpectra** is our effort to extend this spectrum and fill in these gaps.

We drew inspiration from various sources, including the cultural and spiritual depth of indigenous communities. This led us to include new emotions such as "nature_connectedness," "ancestral_reverence," "communal_grief," and "spiritual_awe" ([Proposal for Sentiment Analysis Tool](https://scholarworks.umt.edu/cgi/viewcontent.cgi?article=12880&context=etd)) [25]. These are just some examples of the emotions that we felt were integral to a fuller understanding of humanity.

### Understanding t-SNE and 3D Visualization
**t-Distributed Stochastic Neighbor Embedding (t-SNE)** is a non-linear dimensionality reduction technique that is particularly well-suited for visualizing high-dimensional datasets in low-dimensional spaces, such as 2D or 3D. In our project, t-SNE helps reduce the complexity of emotional data—each represented by several features—into a comprehensible 3D space. This allows us to create an interactive plot that is visually intuitive and easy to interpret. By applying **k-means clustering**, we further categorize the t-SNE-transformed data into different clusters, each representing a unique blend of emotions that humans experience.

These clusters enable us to observe how emotions group together in meaningful ways, providing insight into the relationships between emotions across cultures. We chose to visualize the emotions in 3D to give an enhanced understanding of these connections, showcasing the interplay between various emotional dimensions, namely "Prototypical Emotion Recognition," "Prototypical Emotion Knowledge," and "Advanced Emotion Understanding" ([Prototypical Emotion Recognition](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5679467/)) [23].

### Methodology
1. **Emotion Spectrum**: We compiled an extended list of emotions that go beyond the Eurocentric emotional models, ensuring a culturally-inclusive dataset. The full list consists of 26 emotions, including "gratitude," "tranquility," "resilience," and "family_devotion."

2. **Data Generation and Preprocessing**: We generated additional data samples to create a robust dataset, with emotions randomly selected to ensure balanced representation. We converted the categorical emotion values into numerical dummy variables to prepare the data for dimensionality reduction.

3. **Dimensionality Reduction (t-SNE)**: We employed t-SNE to reduce our high-dimensional emotion data into three components. We set hyperparameters, such as `perplexity` and `n_iter`, to optimize the visualization quality.

4. **Clustering with k-Means**: We applied k-means clustering to group the t-SNE-transformed data into 20 clusters. Each cluster represents a unique subset of emotions, and we visualize these clusters to identify patterns of emotional similarity.

5. **3D Visualization**: We used Plotly to create an interactive 3D scatter plot that allows users to explore how emotions relate to each other. Users can hover over each point to view specific emotions, providing a rich, exploratory experience.

<img width="858" alt="Screenshot 2024-10-09 at 4 07 46 PM" src="https://github.com/user-attachments/assets/3d9ecdc5-b19c-47ac-824e-4ee61f218081">


### Key Insights from Research
- **Inclusion of Indigenous Emotions**: Inspired by the shortcomings of models like Plutchik's, our research highlighted the need to include emotions experienced by indigenous communities, emphasizing spiritual and communal aspects ([Proposal for Sentiment Analysis Tool](https://scholarworks.umt.edu/cgi/viewcontent.cgi?article=12880&context=etd)) [25].

- **Sentiment Analysis Beyond Binary**: Traditional sentiment analysis tools often miss nuances of human emotion by reducing sentiment to simplistic measures like thumbs up/down. Our approach provides a more nuanced understanding, crucial for campaigns and strategies that rely on emotional engagement ([Cambridge Analytica & Sentiment Analysis](https://www.businessinsider.com/cambridge-analytica-whistleblower-christopher-wylie-facebook-data-2019-10)) [25].

- **FATE Principles**: Fairness, Accountability, Transparency, and Ethics (FATE) were central to our project, ensuring unbiased data representation and respecting user privacy ([FATE Principles](https://journals.sagepub.com/doi/10.1177/2053951716679679)) [25].

### Project Structure
- **Data**: The data folder contains generated datasets representing various emotions along with their recognition, knowledge, and understanding metrics.
- **Notebooks**: The Jupyter notebooks include step-by-step procedures for data preprocessing, t-SNE application, clustering, and visualization.
- **Images**: Placeholder for visual representations from our research and clustering results, showcasing the 3D emotional spectrum.

### How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/reyiyama/EmoSpectra.git
   ```
2. Navigate to the project directory:
   ```bash
   cd EmoSpectra
   ```
3. Open the Jupyter notebook and run all cells to see the interactive 3D visualization.

### Applications
**EmoSpectra** has numerous applications, including:
- **Mental Health**: Providing therapists with a broader framework for understanding clients' emotions. Understanding the diversity of emotions can lead to more personalized therapy and enhance emotional well-being by addressing the full spectrum of human experiences. This aligns with the work done by Hume.ai, which aims to provide nuanced emotional data for emotionally intelligent AI systems ([Hume.ai - What is Emotion Science?](https://dev.hume.ai/docs/resources/science#published-research)) [24].

- **Cultural Research**: Enabling anthropologists to visualize and understand emotions from diverse cultural perspectives. By mapping the emotional experiences of various communities, researchers can appreciate both universal and culturally specific expressions, similar to Hume.ai’s findings that show a shared but nuanced expression of emotions across different cultures ([Are Emotional Expressions Universal?](https://dev.hume.ai/docs/resources/science#published-research)) [24].

- **NGOs and Activism**: Assisting NGOs in crafting more resonant campaigns by analyzing community-specific emotional responses. By recognizing nuanced emotions, NGOs can better connect with their audiences, similar to how empathic AI by Hume.ai strives to understand complex human emotions to provide more meaningful interactions ([Can AI "Detect" Emotions?](https://dev.hume.ai/docs/resources/science#published-research)) [24].

### Future Work
- **Expanding Emotion Categories**: Collaborate with cultural experts to further refine and expand the emotion categories. This would be similar to the approach taken by Hume.ai, which emphasizes the high-dimensional nature of emotions and the need to quantify complex semantic spaces to understand the intricacies of emotional experience ([Semantic Space Theory](https://dev.hume.ai/docs/resources/science#published-research)) [24].
![image](https://github.com/user-attachments/assets/60a62da6-4250-4358-98fd-93a1e9c159ea)


- **Improved Clustering**: Experiment with other clustering algorithms, such as DBSCAN, to capture more nuanced relationships between emotions. Incorporating other data-driven approaches like Semantic Space Theory (SST) used by Hume.ai could help in capturing the continuous and blended nature of emotions, offering a more refined emotional mapping ([What is Semantic Space Theory?](https://dev.hume.ai/docs/resources/science#published-research)) [24].
![image](https://github.com/user-attachments/assets/471c6558-c73b-490a-acbf-2c861c37c631)


- **Real-time Data Integration**: Integrate with social media APIs to map real-time emotions and their cultural contexts. Hume.ai’s research on capturing emotional expressions in real-time and across multiple dimensions has demonstrated the importance of recognizing nuanced emotional data, and incorporating such techniques could enhance our real-time emotional mapping capabilities ([Emotion Science and AI](https://dev.hume.ai/docs/resources/science#published-research)) [24].

### Citations
- Plutchik's Wheel of Emotions: [Putting some emotion into your design: Plutchik’s Wheel of Emotions](https://www.interaction-design.org/literature/article/putting-some-emotion-into-your-design-plutchik-s-wheel-of-emotions)
- FATE Principles: [The ethics of algorithms: Mapping the debate](https://journals.sagepub.com/doi/10.1177/2053951716679679)
- Indigenous Emotion Inclusion: [Graham, 2021 - Exploring Community and Nature Connectedness](https://scholarworks.umt.edu/cgi/viewcontent.cgi?article=12880&context=etd)
- Prototypical Emotion Recognition: [Prototypical Emotion Recognition, Knowledge, and Understanding](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5679467/)
- Hume.ai Research: [Hume.ai - What is Emotion Science?](https://dev.hume.ai/docs/resources/science#published-research)

### Contact
For questions, feel free to contact the development team:
- **Tony Smith**: s3972733@student.rmit.edu.au
- **Amay Iyer**: s3970066@student.rmit.edu.au
- **Vikas Vikas**: s3967625@student.rmit.edu.au
- **Tabrez Sheikh**: s3989516@student.rmit.edu.au

We hope that **EmoSpectra** serves as a foundation for further research into sentiment analysis and emotional inclusivity. Let's bring the unspoken emotions of humanity to the forefront and foster greater empathy worldwide.
