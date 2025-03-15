# MusicAnalysis

## Overview
This project explores trends in music listening habits using the **Subset of the Million Song Dataset** from Kaggle. The analysis investigates:
- Genre popularity distribution
- Genre trends over time
- Dynamic interactive visualizations using Plotly

---

## Features
- **Static Analysis**:
  - Genre popularity visualization.
  - Trends of music genres over time.
- **Dynamic Visualizations**:
  - Interactive bar charts and line graphs with Plotly.
- **Custom Genre Mapping**:
  - Manual mapping of artist names to genres.
  - Extended functionality to refine unmapped artists.

---

## Dataset
The dataset used is a subset of the **Million Song Dataset**, sourced from Kaggle: [Subset of the Million Song Dataset](https://www.kaggle.com/datasets/sansastark/subset-of-the-million-song-dataset).


### Preprocessing
To analyze genre trends, artists are mapped to genres using a predefined dictionary. Unmapped artists can be manually reviewed and added to the mapping for accuracy.

---

## Installation and Setup

### Prerequisites
- Python 3.8+
- Libraries:
  - pandas
  - plotly

Install the necessary libraries:
```bash
pip install pandas plotly
```

---

## Key Code Snippets

### Artist-to-Genre Mapping
The `genre_mapping.py` script includes a manually defined dictionary:
```python
# Example mapping
genre_mapping = {
    'The Beatles': 'Rock',
    'Eminem': 'Rap',
    'Taylor Swift': 'Pop',
    # Add more mappings...
}
```
Unmapped artists are identified dynamically and can be logged for further review.

### Interactive Plotly Charts
The notebook uses Plotly for creating interactive visualizations:
```python
# Genre popularity chart
fig = px.bar(
    genre_counts,
    x='Genre',
    y='Count',
    title="Genre Popularity",
    labels={'Count': 'Number of Songs', 'Genre': 'Music Genre'}
)
fig.show()
```

---

## Future Enhancements
- **Dynamic Genre Fetching**:
  - Integrate Spotify API to fetch genres dynamically for unmapped artists.
- **Additional Filters**:
  - Include sliders for year ranges or multi-select dropdowns for multiple genres.
- **Deployment**:
  - Share interactive visualizations via web-hosted notebooks or similar platforms.

---

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

---

## License
This project is licensed under the MIT License.

---

## Contact
For questions or collaboration, contact:
- **Your Name**: your.email@example.com
- GitHub: [yourusername](https://github.com/yourusername)

