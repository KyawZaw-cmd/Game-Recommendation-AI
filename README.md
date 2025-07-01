# Product Recommendation AI

[![Python](https://img.shields.io/badge/Python-3.7%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

A content-based product recommendation system built with Python, designed for use in Google Colab or locally. This project demonstrates how to preprocess product data, perform exploratory data analysis, and build a recommendation engine using TF-IDF and cosine similarity.

## Features

- Cleans and preprocesses product data
- Visualizes product categories and types
- Builds a content-based recommender using product metadata
- Provides recommendations for similar products

## Requirements

- Python 3.7+
- The following Python libraries:
  - numpy
  - pandas
  - matplotlib
  - seaborn
  - plotly
  - scikit-learn

Install the required libraries with:

```bash
pip install numpy pandas matplotlib seaborn plotly scikit-learn
```

## Dataset

The script expects a file named `productlist.csv` in the project directory. This CSV should contain at least the following columns:

- `product` (product name/title)
- `category`
- `sub_category`
- `type`
- `brand` (if available)

**Note:** The `productlist.csv` file is NOT included in this repository. You must provide your own dataset to use the recommender.

## Usage

### In Google Colab

1. Upload your `productlist.csv` to the Colab environment.
2. Upload or copy the contents of `product_recommendation_AI.py` into a Colab notebook cell, or run the notebook version if available.
3. Run the code cells to execute the analysis and generate recommendations.

### Locally

1. Place your `productlist.csv` and `product_recommendation_AI.py` in the same directory.
2. Install the required libraries (see above).
3. Run the script:

```bash
python product_recommendation_AI.py
```

## How it Works

- Loads and cleans the product data.
- Performs exploratory data analysis with visualizations.
- Uses TF-IDF vectorization and cosine similarity to recommend products based on their metadata.
- Improves recommendations by combining multiple metadata fields and cleaning text.

## Example

To get recommendations for a product, use:

```python
get_recommendations('Product Name')
```

or, for the improved recommender:

```python
get_recommendations_2('Product Name')
```

Replace `'Product Name'` with the actual name of a product from your dataset.

## Customization

- You can modify the script to include additional product features.
- Adjust the number of recommendations returned by changing the slicing in the `get_recommendations` functions.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

*This project is for educational purposes. Please ensure you have the right to use any data you provide.* 