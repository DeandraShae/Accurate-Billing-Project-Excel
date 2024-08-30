Project: Ensuring Data Integrity Between Hotel Invoice and Service Provider Records 📊
----------------------------------------------------------------------------------------------------

### Introduction

In this project, I aimed to validate the consistency and accuracy of data recorded by a hotel and a corresponding service provider. Discrepancies in data can lead to financial miscalculations, billing errors, and ultimately, customer dissatisfaction. The primary focus was on matching records related to guest check-ins, durations of stay, daily rates, and total billing amounts.
![image](https://github.com/user-attachments/assets/fc7924c3-4729-46c7-8e66-dd7c76c72b3a)

![image](https://github.com/user-attachments/assets/2c71edcc-6758-46e7-90f4-f9d96773740f)

### Objectives

-   **Verify the accuracy of check-in and check-out dates.** ✔️
-   **Ensure consistency in the number of nights stayed as recorded by both sources.** 🛏️
-   **Confirm the daily room rates and total amounts billed are identical between the two sources.** 💸
-   **Identify and quantify any discrepancies.** 🔍

### Tools and Technologies Used

-   **Microsoft Excel**: Utilized for all data handling, application of formulas for comparison, and visualization of discrepancies. 📈

### Methodology

#### Data Structuring

Data was organized into comparative sets with corresponding fields from both the hotel and the service provider. This structuring was crucial for direct comparison and validation.

#### Formulas Used
![image](https://github.com/user-attachments/assets/3f0129fb-32e9-4fd0-b001-2a428ade452e)

1.  **XLOOKUP**:
    -   `=XLOOKUP(A2, 'Hotel Invoice'!B:B, 'Hotel Invoice'!C:C)`
    -   Purpose: To find and return matching records from the hotel data for validation against the service provider's records.
![image](https://github.com/user-attachments/assets/2377bc12-3dbd-4b59-8a6e-adaba852f7ef)

2.  **COUNTIF**:
    -   `=COUNTIF(range, criteria)`
    -   Purpose: To count the number of discrepancies in check-out dates and total nights stayed across the compared datasets.
  ![image](https://github.com/user-attachments/assets/5ba0fbc1-8707-4a5a-ac70-b20d3407d638)

3.  **SUMPRODUCT**:
    -   `=SUMPRODUCT(--(range1=range2))`
    -   Purpose: To perform conditional counts and sums over arrays, used here to tally discrepancies when comparing nights stayed and total billed amounts.

#### Conditional Formatting

-   Applied to highlight discrepancies in the data directly within Excel, making it easier to identify and address mismatches in real-time. 🎨
![image](https://github.com/user-attachments/assets/2ad8bb4e-2520-4966-b144-75dc59d5e1db)

### Results

-   **Date Discrepancies**: Identified two instances where the check-out dates did not match, leading to further review to correct the records.
-   **Nights Stayed**: Found discrepancies in two records regarding the number of nights stayed, impacting the total billed amount.
-   **Financial Discrepancies**: Uncovered a total financial discrepancy of $220 due to variances in billed amounts, likely from misapplied rates or computational errors.

### Conclusion

This project highlighted the critical need for meticulous data verification and reconciliation practices in hospitality management. Through systematic comparison and the application of advanced Excel functions, I enhanced data reliability, thereby reducing potential financial discrepancies and increasing stakeholder trust.
