# Movie Review Sentiment Analysis

A sentiment analysis project that uses NLTK's VADER (Valence Aware Dictionary and sEntiment Reasoner) to analyze movie reviews from the IMDb dataset and evaluate the sentiment classification performance.

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## 🎯 Overview

This project performs sentiment analysis on movie reviews using NLTK's VADER sentiment analyzer. The goal is to classify movie reviews as positive or negative and compare the results with the original labels to evaluate the model's performance.

The project demonstrates:
- Data preprocessing and cleaning
- Sentiment analysis using VADER
- Performance evaluation using classification metrics
- Challenges in sentiment analysis with real-world data

## ✨ Features

- **Data Loading & Preprocessing**: Loads movie review data and handles missing/blank records
- **VADER Sentiment Analysis**: Utilizes NLTK's VADER for sentiment scoring
- **Performance Evaluation**: Comprehensive analysis using accuracy, precision, recall, and F1-score
- **Confusion Matrix**: Visual representation of classification results
- **Compound Score Analysis**: Converts VADER compound scores to binary sentiment labels

## 📊 Dataset

The project uses a movie reviews dataset containing:
- **Size**: 1,938 reviews (after preprocessing)
- **Format**: Tab-separated values (TSV)
- **Labels**: Binary classification (positive/negative)
- **Source**: IMDb movie reviews dataset

Distribution:
- Positive reviews: 969
- Negative reviews: 969

## 🛠️ Installation

### Prerequisites
- Python 3.6 or higher
- pip package manager

### Required Libraries
```bash
pip install nltk pandas numpy scikit-learn jupyter
```

### NLTK Data Download
```python
import nltk
nltk.download('vader_lexicon')
```

## 🚀 Usage

1. **Clone the repository**:
```bash
git clone https://github.com/mustafasamy28/movie-sentiment-analysis.git
cd movie-sentiment-analysis
```

2. **Install dependencies**:
```bash
pip install -r requirements.txt
```

3. **Run the Jupyter notebook**:
```bash
jupyter notebook Sentiment-Analysis.ipynb
```

4. **Execute the cells** to see the sentiment analysis in action.

## 📈 Results

The VADER sentiment analyzer achieved the following performance metrics:

- **Overall Accuracy**: 77.67%
- **Precision**:
  - Negative: 0.72
  - Positive: 0.78
- **Recall**:
  - Negative: 0.75
  - Positive: 0.83
- **F1-Score**:
  - Negative: 0.69
  - Positive: 0.70

### Key Insights
- VADER shows higher recall for positive sentiment detection
- The model struggles with nuanced movie reviews where positive elements are mentioned before negative conclusions
- Demonstrates the challenge of understanding human semantics in sentiment analysis

## 🔧 Technologies Used

- **Python 3.6+**: Core programming language
- **NLTK**: Natural Language Toolkit for sentiment analysis
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Scikit-learn**: Machine learning metrics and evaluation
- **Jupyter Notebook**: Interactive development environment

## 📁 Project Structure

```
movie-sentiment-analysis/
│
├── Sentiment-Analysis.ipynb    # Main notebook with analysis
├── TextFiles/
│   └── moviereviews.tsv       # Dataset file
├── requirements.txt           # Python dependencies
├── README.md                 # Project documentation
└── LICENSE                   # License file
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Ideas for contributions:
- Implement other sentiment analysis models
- Add data visualization components
- Improve preprocessing techniques
- Add more evaluation metrics

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

**Mostafa Samy**
- 📧 Email: mustafasamy28@gmail.com
- 💼 LinkedIn: [Mostafa Samy](https://www.linkedin.com/in/mostafa-samy-9b95711a7/)
- 🐱 GitHub: [@mustafasamy28](https://github.com/mustafasamy28)

---

⭐ If you found this project helpful, please give it a star on GitHub!

## 🔮 Future Enhancements

- [ ] Implement deep learning models (LSTM, BERT)
- [ ] Add real-time sentiment analysis capability
- [ ] Create a web interface for the sentiment analyzer
- [ ] Expand dataset with more diverse review sources
- [ ] Add sentiment intensity visualization
