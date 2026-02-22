## **Attention Visualizations**


**Overview:**
To better understand how attention works in LLMs, this project builds the Q, K, V matrices from raw input and visualizes attention weights under different circumstances. Instead of using random vectors, we use a short sentence to visualize attention patterns, compare scaled vs. unscaled attention, and analyze how runtime changes with sequence length. The goal is to make the mathematics of attention transparent and interpretable.


**Methods:** I implemented scaled dot-product attention and multi-head self-attention from scratch to directly inspect queries, keys, values, and attention weights. Rather than using random vectors, I embedded a short sentence (English) to produce interpretable heatmaps.


**Key Results:** Multi-head attention produces distinct head behaviors, even on short sentences. Removing scaling results in sharper softmax distributions. Runtime analysis plot was not as I expected (O(n^2)), may require revision. 


**How to Run:** Clone repo, install dependencies, and run in VS Code. Alternatively, download notebook manually and run in Google Colab. 


**Requirements:** Mainly torch and matplotlib are required. All requirements are in the requirements.txt file, and also imported at the first code block in the notebook.
