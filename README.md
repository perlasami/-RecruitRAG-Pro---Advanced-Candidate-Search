# 🚀 RecruitRAG Pro - Advanced Candidate Search

Intelligent resume matching with AI-powered semantic search

![Screenshot](https://github.com/username/repo/blob/main/images/Screenshot_2025-09-04_160726.png?raw=true)


## Overview
RecruitRAG Pro is an intelligent resume matching system that uses AI-powered semantic search to find the perfect candidates for job openings. The system processes resumes, extracts skills and project information, and creates a searchable knowledge base using advanced natural language processing techniques.

## Features
- **AI-Powered Semantic Search**: Find candidates based on meaning rather than just keywords  
- **GitHub Integration**: Automatically fetches and analyzes candidate GitHub projects  
- **Skill Extraction**: Identifies technical skills from resume content  
- **Cosine Similarity Matching**: Advanced vector search for accurate results  
- **Beautiful Web Interface**: Gradio-based UI for easy interaction  
- **Query Enhancement**: Automatically expands search queries for better results  

## Technology Stack
- **Natural Language Processing**: spaCy for text processing  
- **Embeddings**: Sentence Transformers (`all-mpnet-base-v2`)  
- **Vector Search**: FAISS with cosine similarity  
- **Web Framework**: Gradio for the user interface  
- **Data Processing**: Pandas, NumPy  
- **APIs**: GitHub API for live project data  

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/RecruitRAG-Pro.git
cd RecruitRAG-Pro
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Download spaCy model:

```bash
python -m spacy download en_core_web_sm
```

Set up environment variables:  
Create a `.env` file with your GitHub API token:

```text
GITHUB_TOKEN=your_github_token_here
```

## Usage

### Data Processing
- The system processes resume data from the HuggingFace dataset  
- Extracts skills, GitHub profiles, and project information  
- Creates enhanced vector embeddings for semantic search  

### Running the Application
```bash
python recruitrag_app.py
```

### Search Interface
- Enter search queries like `"Machine learning engineer with Python and TensorFlow experience"`  
- Filter results to show only candidates with GitHub portfolios  
- View detailed candidate information with skill matching scores  

## Dataset
The system uses the **Resume-Screening-Dataset** from HuggingFace, which contains resumes labeled with job roles and decision outcomes.

## How It Works
1. **Resume Processing**: Cleans and extracts information from resumes  
2. **Skill Extraction**: Identifies technical skills using NLP techniques  
3. **GitHub Integration**: Fetches live project data from GitHub profiles  
4. **Vector Embedding**: Creates semantic embeddings of resume content  
5. **Indexing**: Builds a FAISS index for efficient similarity search  
6. **Query Processing**: Enhances and expands user queries for better matching  
7. **Search & Ranking**: Finds and ranks candidates based on semantic similarity  

## Project Structure
```
RecruitRAG-Pro/
├── data_processing.py    # Resume processing and embedding
├── search_system.py      # Search functionality
├── recruitrag_app.py     # Main application
├── requirements.txt      # Dependencies
├── README.md             # This file
└── images/               # Screenshots
    ├── Screenshot_2025-09-04_160726.png
    ├── Screenshot_2025-09-04_160740.png
    └── Screenshot_2025-09-04_160801.png
```

## Results
The system provides:
- Percentage match scores for each candidate  
- Highlighted relevant experience sections  
- GitHub project information when available  
- Skills overview for each candidate  
- Clean, professional presentation of results  

## Future Enhancements
- Integration with LinkedIn profiles  
- Advanced filtering options  
- Batch processing of multiple queries  
- Export functionality for candidate shortlists  
- Integration with applicant tracking systems  

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- HuggingFace for the resume dataset  
- Facebook AI Research for FAISS  
- UKPLab for Sentence Transformers  
- GitHub for their API  
