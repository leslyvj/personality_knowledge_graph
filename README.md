# Personality Knowledge Graph

An NLP-powered knowledge graph builder that extracts entities, personality traits, and relationships from text to create interactive visualizations.

## About The Project

This project demonstrates how to build a personality-focused knowledge graph using natural language processing techniques. It extracts named entities, analyzes personality traits through sentiment analysis and adjective extraction, and visualizes the relationships between entities in an interactive graph format.

The system processes text data to identify people and organizations, assigns personality characteristics based on linguistic patterns, and creates a network graph showing how different entities are connected through co-occurrence in text.

### Built With

* [![Python][Python.badge]][Python-url]
* [![spaCy][spaCy.badge]][spaCy-url]
* [![NetworkX][NetworkX.badge]][NetworkX-url]
* [![Matplotlib][Matplotlib.badge]][Matplotlib-url]

## Getting Started

Follow these steps to set up and run the personality knowledge graph builder locally.

### Prerequisites

Ensure you have Python 3.7+ installed on your system.

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/leslyvj/personality_knowledge_graph.git
   ```

2. Install required packages
   ```sh
   pip install spacy textblob networkx matplotlib pyvis
   ```

3. Download the spaCy language model
   ```sh
   python -m spacy download en_core_web_sm
   ```

4. Open the Jupyter notebook
   ```sh
   jupyter notebook personality_knowledge_graph.ipynb
   ```

## Usage

The notebook processes text to build knowledge graphs with personality insights:

1. **Entity Extraction**: Identifies people, organizations, and locations using spaCy's NER
2. **Personality Analysis**: Extracts personality traits through adjective detection and sentiment analysis
3. **Graph Construction**: Builds a network graph based on entity co-occurrence
4. **Visualization**: Creates both static (matplotlib) and interactive (PyVis) visualizations

### Example Input
```python
text = """
Elon Musk, a bold and risk-taking entrepreneur, founded SpaceX and leads Tesla.
Under his leadership, SpaceX aims to colonize Mars.
Meanwhile, Jeff Bezos, a methodical and ambitious thinker, founded Blue Origin to explore space too.
"""
```

### Output
The system generates:
- Entity list with classifications (PERSON, ORG, LOC)
- Personality trait mappings for each person
- Interactive HTML graph visualization
- Static matplotlib network diagram

## Features

- **Named Entity Recognition**: Automatically identifies and classifies entities in text
- **Personality Trait Extraction**: Uses adjectives and sentiment analysis to infer personality characteristics
- **Relationship Mapping**: Discovers connections between entities through co-occurrence analysis
- **Interactive Visualization**: Creates explorable network graphs with PyVis
- **Color-coded Nodes**: Visual distinction between person, organization, and location entities

## Roadmap

- [ ] Add support for more sophisticated personality models
- [ ] Implement custom relationship extraction beyond co-occurrence
- [ ] Add export functionality for graph data
- [ ] Support for multiple languages
- [ ] Integration with larger text corpora

## Contributing

Contributions are what make the open source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

## Contact

Lesly V J - [@vj_lesly](https://x.com/vj_lesly) - lesly.ds24@duk.ac.in

Project Link: [https://github.com/leslyvj/personality_knowledge_graph](https://github.com/leslyvj/personality_knowledge_graph)

## Acknowledgments

* [spaCy Documentation](https://spacy.io/usage)
* [NetworkX Documentation](https://networkx.org/documentation/stable/)
* [PyVis Network Visualization](https://pyvis.readthedocs.io/)
* [TextBlob Sentiment Analysis](https://textblob.readthedocs.io/)
* [Best README Template](https://github.com/othneildrew/Best-README-Template)

<!-- MARKDOWN LINKS & IMAGES -->
[Python.badge]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
[Python-url]: https://python.org/
[spaCy.badge]: https://img.shields.io/badge/spaCy-09A3D5?style=for-the-badge&logo=spacy&logoColor=white
[spaCy-url]: https://spacy.io/
[NetworkX.badge]: https://img.shields.io/badge/NetworkX-FF6B6B?style=for-the-badge&logo=python&logoColor=white
[NetworkX-url]: https://networkx.org/
[Matplotlib.badge]: https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white
[Matplotlib-url]: https://matplotlib.org/
