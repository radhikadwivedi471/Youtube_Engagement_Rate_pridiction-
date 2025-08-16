# Youtube_Engagement_Rate_pridiction-
Multimodal deep learning project to predict YouTube video engagement rate using a combination of text, tabular, and image data, with additional GNN enhancement.
Engagement Rate Formula: Engagement\ Rate = likes + comment_count\view_count 

1. Data Preprocessing:
Clean missing or invalid values.
Convert publishedAt & trending_date to datetime features.
Extract text features from title, tags, description.
Extract tabular features: view_count, likes, dislikes, comment_count, categoryId.
Download thumbnail images locally using thumbnail_link before processing.

2. Image Feature Extraction:
Use CLIP or YOLO for extracting image embeddings from thumbnails.

3. Text Feature Extraction:
Tokenize and pad sequences for captions (title, description, tags).

4. Graph Neural Network (GNN) Enhancement:
Build a graph where nodes are videos and edges are based on similarity (same categoryId, similar tags, or same channelId).
Use GNN to propagate features across similar videos for richer representations.

5. Model Architectures:
Text-only model (LSTM or Transformer-based).
Tabular-only model (Dense layers).
Image-only model (CNN-based).

Multimodal model:
Early fusion (combine before hidden layers).
Late fusion (combine outputs of separate models).
Hybrid fusion (mix of early and late).

6.Result
Built text, tabular, and image pipelines,
Implements GNN enhancement.
Trains models and compares them visually.
Takes YouTube link as input for prediction.








