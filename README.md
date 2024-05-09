DESCRIPTION:

Training Data: https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023?resource=download

The flight app search and visualization tool is a Python package designed to facilitate flight search and visualization using data from RapidAPI's TripAdvisor API and predictions from an Azure ML API endpoint which is a Boosted Regression Tree model for this example (you will have to model your data in azure seperately). This tool serves as a user-friendly interface for searching and visualizing flight details based on specified criteria. Users can input parameters such as source and destination airports, departure date, class of service, and sort order. The application connects to RapidAPI's TripAdvisor API to fetch relevant flight data, which is then processed and displayed through a Streamlit web app. Additionally, the tool utilizes an Azure ML API endpoint to predict arrival delays for the fetched flights, enhancing the user experience by providing estimated delay information alongside other flight details. Estimated delay can be represented in negative numbers which means the flight is usually early, or in positive numbers which reflects a delay in minutes. 

INSTALLATION:

If you would like to locally run the app, you can:

1. Create and deploy whichever machine learning model you would like using Azure ML. 
2. Download the .py file from github.
3. Ensure you have Python installed on your system. If not, download and install Python from the official website (https://www.python.org/).
4. Open a command prompt or terminal window.
5. Navigate to the directory where the `flight_app.py` file is located using the `cd` command.
6. Optionally, create and activate a virtual environment:
   - Create: `python -m venv venv`
   - Activate (Windows): `venv\Scripts\activate`
   - Activate (Linux/Mac): `source venv/bin/activate`
7. Install the required dependencies using pip:

   ```pip install streamlit pandas requests altair```

8. Ensure you have the necessary API keys for accessing RapidAPI's TripAdvisor API and the Azure ML API endpoint. 

EXECUTION:

1. After completing the installation steps, navigate to the directory where the `flight_app.py` file is located in your command prompt or terminal.
2. Run the Streamlit app by executing the following command:

   ```streamlit run flight_app.py```

3. Once the command is executed, the Streamlit app will start running locally.
4. Access the application by opening a web browser and entering the provided URL (usually http://localhost:8501).
5. Input your desired parameters such as source and destination airports, departure date, class of service, and sort order.
6. Click the "Search Flights" button to fetch and display flight details along with predicted delays.
7. Explore the results, including structured flight details and interactive visualizations.
8. You can click on the dots on the graph to navigate to the flight booking website.

Note: Ensure you have a stable internet connection to fetch flight data from RapidAPI's TripAdvisor API and to access the Azure ML API endpoint for predicting arrival delays. Additionally, make sure the necessary API keys are properly configured in the `flight_app.py` script.
