# loan_qualifier_app
Challenge 2


This is a python command-line interface application that allows users to see qualifying loans from lenders quickly and easily. The application works by taking in a `daily_rate_sheet` of loan criteria from various loan providers, asking the user a number of questions to evaluate their loan eligibility, and then returning to them a list of qualifying loans.

---

## Technologies

This project leverages python 3.10 with the following packages:

* [fire](https://github.com/google/python-fire) - For the command line interface, help page, and entrypoint.

* [questionary](https://github.com/tmbo/questionary) - For interactive user prompts and dialogs

---

## Installation Guide

Before running the application first install the following dependencies.

```python
  pip install fire
  pip install questionary
```
![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/image_screenshots/pip_install_fire.png)

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/image_screenshots/pip_install_questionary.png)


---

## Usage

To use the loan qualifier application simply clone the repository and run the **app.py** with:

```python
python app.py
```

## Activity

Upon launching the loan qualifier application you will be greeted with the following prompts.

* Define the new `get_applicant_info()` function.
* Prompt dialog to get the applicant's financial information.
* Inside `get_applicant_info()`, set the `credit_score` variable using the Questionary `text()` syntax. Repeat this step for the `debt`, `income`, `loan_amount`, and `home_value` variables.
* Right now, all values received through Questionary will be set to the type `string`, but the values must be set to `float` to perform floating-point arithmetic. So convert the credit score to `integer` and the rest of the values to `float`
* Inside the `get_applicant_info()` function, write the statement that will return all of the variables.

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/image_screenshots/get_applicant_info.png)

* Find qualifying loans, determine which loans the user are qualifies for.
* Calculate the monthly debt ratio, loan to value ration.
* Filter max loan size, credit score, debt to income and loan to value.
* Use for loop and if statement function.

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/image_screenshots/find_qualifying_loans.png)

* Save csv file from the file path from path provided.
* Set the header and create a csvwriter using csv libray.
* Use the csv library and 'csv.writer' to wire the header row and qualifiying loans.

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/image_screenshots/save_csv_file_path.png)

* Save qualifying loans to a csv file.
* Prompt dialog to ask user's about to save their qualifying loans.
* Use questionary.confirm.ask() to get the user's answer.
* Find if this file is included .csv, if this is included don't save or print .csv in file name,otherwise save oe print .csv in file name.
* Prompt dialog to ask user's what kind of name they wanted to named their qualifying loans file name.
* Use if else statement and find function to save csv file name.
* print the message to confrim the user's requirement.

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/image_screenshots/save_qualifying_loans.png)

* Running the script to the main function. 

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/image_screenshots/main_function_for_running_the_script.png)

* Screenshots image: Testing user's loan_qualifier_app (Zillow_loan.csv)

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/image_screenshots/Loan_qualifier_app.png)

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/Zillow_loan.csv)

* Screenshots image: Testing user's qualifying loans saved file and file name. (Khaing_loans.csv)

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/image_screenshots/Qualifying_loans_saved_file.png)

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/Khaing_loan.csv)

* Screenshots image: Testing user's qualifying loans un-saved file.

![alt text](https://github.com/Khaingz/loan_qualifier_app/blob/main/image_screenshots/Qualifying_loans_non_saved_file.png)


---

## Contributors

Brought to you by Khaing Home Loans.

---

## License

UW
