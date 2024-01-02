
# Time-Series Analysis: Making Series Stationary

This project is focused on analyzing time-series data to determine stationarity and apply transformations to achieve stationarity if necessary. Stationarity is a key concept in time-series analysis, and it is often a requirement for many statistical models like ARIMA.

## Project Structure

- `data/`: Contains the training and validation datasets.
- `notebook/`: Jupyter notebooks for exploratory data analysis and interactive methodology demonstration.
- `scripts/`: Contains Python scripts for checking the stationarity of the series.
- `.gitignore`: The gitignore file to exclude certain files and directories from git version control.
- `requirements.txt`: Lists the dependencies necessary to run the project.

## Dependencies

The project requires the following Python libraries:

- pandas: For data manipulation and analysis.
- numpy: For numerical computing.
- matplotlib: For plotting and visualization.
- scikit-learn: For machine learning and statistical modeling.
- statsmodels: For implementing statistical models.

To install these dependencies, run the following command:

```
pip install -r requirements.txt
```

## Analysis Workflow

1. **Data Loading**: The training and validation datasets are loaded into pandas DataFrames from the CSV files located in the `data/` directory.

2. **Preprocessing**: The 'Date' column is converted to datetime objects, and the DataFrames are indexed on this column for time-series analysis.

3. **Visualization**: The training and validation data are plotted to visualize the count over time.

4. **Stationarity Checks**: The Dickey-Fuller and KPSS tests are applied to the 'count' column to check for stationarity.

5. **Making Series Stationary**:
   - **Differencing**: The first difference of the 'count' column is calculated and plotted to visualize stationarity.
   - **Log Transformation**: The logarithm of the 'count' column is taken, followed by differencing to stabilize variance and mean.

6. **Results Interpretation**: The results of the Dickey-Fuller and KPSS tests after transformations are provided to confirm stationarity.

## Running the Analysis

To run the analysis, navigate to the `scripts/` directory and execute the Python script:

```
python time_series_check_series_stationary
```

Alternatively, you can explore the methodology in an interactive way by opening the Jupyter notebook:

```
jupyter notebook notebook/Making_series_stationary.ipynb
```

## Contribution

Feel free to fork this repository, make changes, and submit pull requests. If you encounter any issues or have any suggestions, please open an issue in the repository.

## License

This project is open source and available under the MIT License.
```
