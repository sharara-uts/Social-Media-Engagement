# Social-Media-Engagement
# Project 1 — Social Media Engagement Analysis (Portfolio)

**Goal:** Find which post type (video, photo, status, link) gets the highest engagement and learn simple data science skills: cleaning, EDA, charts, and insights.

## 1) Dataset
- File: `Live.csv` (7050 rows × 13 columns)
- Columns: reactions (`num_reactions`, `num_comments`, `num_shares`, `num_likes`, `num_loves`, `num_wows`, `num_hahas`, `num_sads`, `num_angrys`) and post types (`status_type_link`, `status_type_photo`, `status_type_status`, `status_type_video`).
- Values are normalized between 0 and 1 (proportions).

> If your CSV is large, you can **not** upload it and instead point to the source. For this project, uploading is OK.

## 2) What I Did (Short Steps)
1. Loaded data in a Jupyter/Colab notebook.
2. Created a single `Post_Type` column from the one-hot columns.
3. Calculated `Total_Engagement` per post and an `Engagement_Score` (weighted: comments×2, shares×3).
4. Answered key questions:
   - Which post type gets the most engagement?
   - Which reaction type is most common?
   - Are likes and shares related? (correlation)
   - What do all reactions look like together? (correlation heatmap)
5. Made clean charts for each answer.
6. Wrote simple, clear insights.

## 3) How to Reproduce
**Option A — Google Colab (easy)**
1. Open the notebook `SocialMedia_Analysis.ipynb` in Colab.
2. Upload `Live.csv` when asked in the notebook.
3. Run all cells.

**Option B — Local (Python 3.10+)**
```bash
pip install -r requirements.txt
python -m notebook  # or jupyter lab / vscode
