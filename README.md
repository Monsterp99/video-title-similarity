# video-title-similarity
AI-Powered Video Title Similarity &amp; Performance Analyzer
**How This Code Works**

This code was created using ChatGPT Open AI assistance. This script analyzes video titles by leveraging AI-powered natural language processing (NLP) to detect similarities and identify low-performing content. It integrates performance normalization, semantic similarity modeling, and data visualization to support content optimization.

1. **Data Preprocessing**

 - Loads a structured dataset containing video titles and key performance metrics.
 - Converts time-based metrics (e.g., "Average View Duration") into numeric values for standardization.
 - Applies MinMaxScaler to normalize performance metrics, ensuring consistent comparisons across different scales.

2. **Performance Evaluation**

 - Computes a weighted performance score based on engagement signals (views, watch time, average percentage viewed, and subscriber impact).
 - Sorts video titles from lowest to highest performance, identifying underperforming content.

3. **Semantic Similarity Analysis**

 - Uses Sentence Transformers (all-MiniLM-L6-v2) to generate vectorized embeddings of each video title.
 - Computes cosine similarity scores between all video titles, creating a semantic similarity matrix.
 - Identifies the most textually similar title for each low-performing video, helping to detect redundant content or overlapping topics.

4. **Visualization & Output**

 - Generates a heatmap to visually represent title similarity relationships.
 - Exports a structured CSV file mapping low-performing titles to their closest semantic matches for further review.

 This process streamlines content audits, topic clustering, and SEO-driven content refinements, ensuring that redundant or underperforming assets can be optimized effectively.
