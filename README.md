# Surgical Outcome Analysis

This project analyzes surgical outcome data to explore cost, profit, and resource usage in surgical procedures. The analysis includes advanced SQL queries, visualizations, and a machine learning model for prediction.

## Project Setup

1. **Environment Setup**:
   - Create and activate a conda environment:
     ```bash
     conda create -n SurgicalOutcomeAnalysis python=3.8
     conda activate SurgicalOutcomeAnalysis
     ```
   - Install the required libraries:
     ```bash
     pip install pandas matplotlib seaborn SQLAlchemy scikit-learn pyodbc
     ```

2. **Database Setup**:
   - Download the `GeneralHospital.bak` file from the following link:
     [General Hospital SQL Server BAK file](https://community.qlik.com/t5/Healthcare/General-Hospital-SQL-Server-BAK-file/td-p/1493132) by Dalton_Ruer.
   - Restore the `GeneralHospital` database using the downloaded `.bak` file:
     ```sql
     RESTORE DATABASE GeneralHospital
     FROM DISK = 'path_to_your_GeneralHospital.bak'
     WITH MOVE 'GeneralHospital_Data' TO 'C:\Program Files\Microsoft SQL Server\MSSQL15.MSSQLSERVER\MSSQL\DATA\GeneralHospital.mdf',
          MOVE 'GeneralHospital_Log' TO 'C:\Program Files\Microsoft SQL Server\MSSQL15.MSSQLSERVER\MSSQL\DATA\GeneralHospital.ldf',
          REPLACE
     ```

3. **Running the Analysis**:
   - Open `SurgicalOutcomeAnalysis.ipynb` in DataSpell.
   - Execute each cell sequentially to perform the analysis and visualizations.

## Project Structure

- `SurgicalOutcomeAnalysis.ipynb`: Jupyter Notebook with data analysis, visualizations, and machine learning model.
- `README.md`: Project documentation.

## License

This project is licensed under the MIT License.

## Acknowledgments

The `GeneralHospital.bak` file is provided by Dalton_Ruer on the Qlik Community Healthcare page or can be downloaded from [here](https://community.qlik.com/t5/Healthcare/General-Hospital-SQL-Server-BAK-file/td-p/1493132).

**Link:** (https://community.qlik.com/t5/Healthcare/General-Hospital-SQL-Server-BAK-file/td-p/1493132)
