# Score_Predictor

**Overview**
This project aims to predict the outcomes of IPL matches using machine learning. The dataset comprises detailed match summaries and ball-by-ball delivery information, which are processed and analyzed to forecast match results. The core of the project is built using a Jupyter notebook (match.ipynb), which is used to develop, train, and export the predictive model as a pickle file. This model is then deployed through a web interface created with Streamlit in PyCharm, allowing users to interact with the model and make predictions in real time.
File Structure**
**	•	matches.csv: Contains summaries of each match including details like match date, teams, score, and outcome.
	•	deliveries.csv: Provides ball-by-ball action of each match, detailing each delivery's outcomes, such as runs scored, wickets taken, etc.
	•	match.ipynb: A Jupyter notebook that contains the data preprocessing, feature engineering, model training, and exporting the model to a pickle file.
	•	pipe.pkl: A pickle file that contains the serialized form of the trained machine learning model.
	•	application.py: A Python file within a PyCharm project that contains the Streamlit code to create a user interface for the model.
**Setup and Installation**
**	1	Python Environment:** Ensure that Python is installed on your system. This project was developed using Python 3.8.
**	2	Library Versions: **It is crucial that the scikit-learn library versions match in both the Jupyter notebook and the PyCharm project environments to avoid any compatibility issues with the pickle file. If there are discrepancies in the versions, update the libraries to match each other.
**	3	Dependencies Installation:**
	•	Install necessary libraries for the Jupyter notebook using: pip install numpy pandas matplotlib seaborn scikit-learn jupyter  
	•	For the PyCharm project with the Streamlit interface, install: pip install streamlit pickle  
**	4	Running the Jupyter Notebook:**
	•	Navigate to the directory containing match.ipynb and run the notebook cells sequentially to process the data, train the model, and generate the pipe.pkl file.
**	5	Setting up the PyCharm Project:**
	•	Ensure that application.py and pipe.pkl are placed in the root of the PyCharm project directory.
	•	Open the terminal within PyCharm.
**	6	Launching the Web Interface:**
	•	In the PyCharm terminal, execute the following command to start the Streamlit web interface: streamlit run application.py  
	•	This command will start the server and the interface will be accessible through a web browser at the local address provided by Streamlit (typically http://localhost:8501).
Usage
Once the web interface is running, users can interact with the model through the Streamlit interface. Input the required parameters as per the match conditions, and the model will predict the outcome based on the data provided.
Support
For any issues regarding setup, version compatibility, or running the application, please refer to the documentation of the respective libraries or feel free to raise an issue in the project repository.
This README provides a comprehensive guide to getting the IPL Match Outcome Prediction project set up and running on your local machine. By following these instructions, users can seamlessly predict outcomes of IPL matches using the developed machine learning model.
