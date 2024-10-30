# Nairobi Office Price Prediction

This project demonstrates the implementation of a simple linear regression model using gradient descent to predict office prices based on office size. The dataset used contains various features, but we will focus on the `SIZE` (office size) and `PRICE` (office price) columns.

## Project Structure

- `.gitignore`: Specifies files and directories to be ignored by Git.
- `data.csv`: The dataset containing office features and prices.
- `main.ipynb`: Jupyter notebook containing the implementation of the linear regression model.
- `venv/`: Virtual environment directory containing all the dependencies.

## Dataset

The dataset is loaded from `data.csv` and contains the following columns:

- `LOC`: Location of the office
- `FUR`: Whether the office is furnished
- `AMB`: Ambiance of the office
- `PROX_SCH`: Proximity to schools
- `PROX_ROAD`: Proximity to roads
- `PROX_MALL`: Proximity to malls
- `WATER`: Availability of water
- `HK_SER`: Availability of housekeeping services
- `SIZE`: Size of the office in square feet
- `PRICE`: Price of the office

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/LancemDev/nairobi-office-price-prediction
    cd nairobi-office-price-prediction
    ```

2. Create and activate a virtual environment:
    ```sh
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate` and for fish use `source venv/bin/activate.fish`
    ```

3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. Open the Jupyter notebook:
    ```sh
    jupyter notebook main.ipynb
    ```

2. Run the cells in the notebook to load the data, train the model, and visualize the results.

## Notebook Overview

### Loading the Data

We load the dataset from `data.csv` and extract the `SIZE` and `PRICE` columns for our analysis.

### Mean Squared Error Function

We define a function to compute the Mean Squared Error (MSE), which will be used as our performance measure technique.

### Gradient Descent Function

We define a function to perform gradient descent, which will be used as our learning algorithm to update the weights (slope and intercept) of our linear regression model.

### Training the Model

We initialize random values for the slope (`m`) and y-intercept (`c`) and train the model for 10 epochs. The error is displayed for each epoch.

### Plotting the Line of Best Fit

After training the model, we plot the line of best fit along with the data points to visualize the results.

### Prediction

Finally, we use the trained model to predict the office price for an office size of 100 square feet.

## Conclusion

This project demonstrates a simple implementation of linear regression using gradient descent. The model is trained on a small dataset and provides a basic understanding of how linear regression works.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.