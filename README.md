
#  Bollywood Gender Stereotype Analysis (2008–2017)

This project identifies and quantifies gender stereotypes in Bollywood movies through text and visual analysis of scripts, trailers, and metadata.

---

## Folder Structure

```
Bollywood-Data-Master/
├── main.ipynb                 # Main analysis notebo
├── processed_scripts_nlp.csv  # NLP-processed movie scripts
├── scripts-text/              # Raw movie scripts (.txt files)
├── wikipedia_data/            # Coref plots, gender lexicons, mentions, centrality
├── visual-data/
│   ├── complete-data.csv      # Gender & emotion data per frame from trailers
│   ├── trailers_list.csv      # Metadata of all trailers
│   └── individual-trailer-data/
├── songsDB.csv                # Song data by singer & gender
├── songsFrequency.csv         # Male/female song frequency by movie
├── cast_gender.csv            # Character-to-gender mapping
├── male_mentions_centrality.csv
├── female_mentions_centrality.csv
```

---

## Objectives

1. **Detect Gender Bias** from both **scripts** and **trailers**.
2. **Quantify Bias** at character, movie, and decade levels.
3. Use **linguistic lexicons** and **centrality metrics** to surface gender-based stereotype patterns.
4. **Visualize Bias** through emotion, screen time, and song allocation analysis.
5. Provide a **Bias Feedback Report** for writers and directors.

---

## ⚙️ Features Implemented

| Subtask | Description |
|--------|-------------|
| **1. Data Cleaning** | Scripts tokenized, POS-tagged, coref-resolved |
| **2. Character Matching** | Characters matched using cast-gender and mention-centrality files |
| **3. Gender Lexicon Analysis** | Adjectives/verbs tagged from male/female lexicons |
| **4. Dependency Parsing** | Extract subject-verb-object patterns to analyze traits linked to gender |
| **5. Screen Time Analysis** | From `complete-data.csv` |
| **6. Emotion Bias** | Plotted emotion distributions by gender |
| **7. Music Bias** | Compared male/female singers using `songsDB.csv` and `songsFrequency.csv` |
| **8. Plot Mentions** | Used `coref_plot.csv` and plot-based mentions |
| **9. Centrality** | Centrality boxplots by gender using mention files |
| **10. Final Output** | Summarized gender stereotypes and visualized them in `main.ipynb` |

---

##  How to Run

1. Clone the repo and navigate into it:
   ```bash
   git clone https://github.com/your-username/Bollywood-Data-Project.git
   cd Bollywood-Data-Project
   ```

2. Ensure the following files/folders are present:
   - `Bollywood-Data-Master/` (contains `main.ipynb`)
   - All CSV datasets and script text files

3. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the notebook:
   ```bash
   jupyter notebook Bollywood-Data-Master/main.ipynb
   ```

---

##  Sample Visualizations

- Boxplots for **Character Centrality by Gender**
- Bar charts of **Emotion Distribution in Trailers**
- Line graphs showing **Screen Time Trends by Gender**
- Heatmaps of **Adjective/Verb Usage Patterns**
- Gender Split of **Songs Per Film**

---

## Contributing

Feel free to fork and submit pull requests for improvements or new insights!

---

## License

This project is under the MIT License.

---

## Maintained By

- **Prashasti Priya**

Feel free to reach out for improvements, collaborations, or issues!
