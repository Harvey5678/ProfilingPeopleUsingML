# Profile People Using Social Media
 
 This application uses transformer-based models to profile people based on social media data by finding similar users. It utilizes a combination of NLP models and Pinecone, a vector database for storing and querying the embeddings created by these models.

The application is structured as a Streamlit web application which provides a user-friendly interface. It allows users to select a model and its tokenizer, set the number of database rows to embed, set the number of similar results to display, and view the embeddings.

## Getting Started

#### Prerequisites
You will need Python 3.7+ installed on your machine. Also, it is recommended to create a virtual environment to avoid conflicts with other packages.

#### Installation
To install all the required Python libraries, navigate to the project root directory and run the following command:

    python -m pip --no-cache-dir install -r .\requirements.txt

#### To run the Streamlit application, navigate to Src/Streamlit directory, then run the following command in your terminal:
```streamlit run Home.py```

## Project Structure
The project structure is as follows:

- Src : This directory contains the current working version of the project.
- Src/Streamlit : This directory contains the Streamlit application files.
- Src/Streamlit/Home.py : This is the main script for running the Streamlit application.
- Src/model_class.py : This Python module defines the model class used in the application.
- Src/system_logging.py : This Python module defines the system logging class used in the application.
- docs : This directory contains documentation and scripts relevant to the project.
- features : This directory includes features that have not yet been implemented into a working version. Additionally, it includes test versions of these features as individual components.
## How It Works
Upon running the application, users can select a model and its tokenizer, set the number of database rows to embed and the number of similar results to display. Once the "Embed Data" button is clicked, the chosen data is embedded and uploaded to Pinecone and the logger. The embeddings can then be viewed directly on the application interface.

The application uses the model_class.py and system_logging.py modules for its operations. The model_class.py module defines the Model class, which is used to handle the transformer models used for embedding. The system_logging.py module defines the SystemLogging class, which logs the system's operations.

## Future Work
Future work involves the implementation of additional features that have not yet been incorporated into the working version of the application. We plan to expand different types of social media attributes, implement ranking, and experiment with a similarity metric for embedding evaluation.

## Feedback
If you have any feedback or run into issues, please file an issue on this GitHub repository.
