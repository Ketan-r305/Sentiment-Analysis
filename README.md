# Model Evaluation and Validation
## Project: Predicting Housing Maintenance Fines

### Install

This project requires **Miniconda/Anaconda** installed on your system:

<!-- - [NumPy](http://www.numpy.org/) -->
<!-- - [Pandas](http://pandas.pydata.org/) -->
<!-- - [matplotlib](http://matplotlib.org/) -->
<!-- - [scikit-learn](http://scikit-learn.org/stable/) -->
After successfully installing **Miniconda/Anaconda** on your system.

In the base environment, install jupyter notebook using conda package number.

Clone this repository on your system.

Navigate to this folder in the **Miniconda/Anaconda** shell.

Then, run conda env create -f environment.yml. This will create the required environment.

Launch the jupyter-notebook from the base environment and then select the environment in the notebook and
run the notebook **main.ipynb**

<!-- You will also need to have software installed to run and execute a [Jupyter Notebook](http://jupyter.org/install.html). -->

<!-- If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](https://www.anaconda.com/download/) distribution of Python, which already has the above packages and more included. -->

### Files

<!-- Template code is provided in the `boston_housing.ipynb` notebook file. You will also be required to use the included `visuals.py` Python file and the `housing.csv` dataset file to complete your work. While some code has already been implemented to get you started, you will need to implement additional functionality when requested to successfully complete the project. Note that the code included in `visuals.py` is meant to be used out-of-the-box and not intended for students to manipulate. If you are interested in how the visualizations are created in the notebook, please feel free to explore this Python file. -->
dataset folder contains the dataset.

main.ipynb has all the code in it.

environment.yml contains the required production environment for the project.

### Results

Performance of Logistic Regression model on the dataset based on autograder is the best.

roc_auc_score for the trained model is 0.75.


<!-- ### Run

In a terminal or command window, navigate to the top-level project directory `boston_housing/` (that contains this README) and run one of the following commands:

```bash
ipython notebook boston_housing.ipynb
```
or
```bash
jupyter notebook boston_housing.ipynb
```
or open with Juoyter Lab
```bash
jupyter lab
```

This will open the Jupyter Notebook software and project file in your browser. -->

### Data

The Michigan Data Science Team ([MDST](http://midas.umich.edu/mdst/)) and the Michigan Student Symposium for Interdisciplinary Statistical Sciences ([MSSISS](https://sites.lsa.umich.edu/mssiss/)) have partnered with the City of Detroit to help solve one of the most pressing problems facing Detroit - blight. [Blight violations](http://www.detroitmi.gov/How-Do-I/Report/Blight-Complaint-FAQs) are issued by the city to individuals who allow their properties to remain in a deteriorated condition. Every year, the city of Detroit issues millions of dollars in fines to residents and every year, many of these fines remain unpaid. Enforcing unpaid blight fines is a costly and tedious process, so the city wants to know: how can we increase blight ticket compliance?

**Features**

1. `ticket_id`: unique identifier for tickets

2. `agency_name`: Agency that issued the ticket

3. `inspector_name`: Name of inspector that issued the ticket

4. `violator_name`: Name of the person/organization that the ticket was issued to

5. `violation_street_number`, `violation_street_name`, `violation_zip_code`: Address where the violation occurred

6. `mailing_address_str_number`, `mailing_address_str_name`, `city`, `state`, `zip_code`, `non_us_str_code`, `country`: Mailing address of the violator

7. `ticket_issued_date`: Date and time the ticket was issued

8. `hearing_date`: Date and time the violator's hearing was scheduled

9. `violation_code`, `violation_description`: Type of violation

10. `disposition`: Judgment and judgement type

11. `fine_amount`: Violation fine amount, excluding fees

12. `admin_fee`: $20 fee assigned to responsible judgments

13. `state_fee`: $10 fee assigned to responsible judgments

14. `late_fee`: 10% fee assigned to responsible judgments

15. `discount_amount`: discount applied, if any

16. `clean_up_cost`: DPW clean-up or graffiti removal cost

17. `judgment_amount`: Sum of all fines and fees

18. `grafitti_status`: Flag for graffiti violations

19. `payment_amount`: Amount paid, if any

20. `payment_date`: Date payment was made, if it was received

21. `payment_status`: Current payment status as of Feb 1 2017

22. `balance_due`: Fines and fees still owed

23. `collection_status`: Flag for payments in collections


**Target Variable**
<!-- 4. `MEDV`: median value of owner-occupied homes -->

24. compliance [target variable for prediction]

        Null = Not responsible

        0 = Responsible, non-compliant

        1 = Responsible, compliant

        compliance_detail - More information on why each ticket was marked compliant or non-compliant
