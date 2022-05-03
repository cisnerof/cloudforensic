# Mega Extraction

## Disclaimer
This guide serves as my personal reference. Do your own test for feasibility of your deployment.
All Access must be legal or authorized.

## Features of Mega
- MEGA’s outstanding feature is its end-to-end encryption. All files that are uploaded to MEGA’s servers are encrypted on the side of the client, meaning the user is the only one who can decrypt their own data. 
- Apart from encryption, MEGA has plenty of such as chat client. 
- Everything uploaded to MEGA is encrypted with an individual encryption key, which can be sent separately.
- Paid users can set expiration dates and passwords for the links.

## Free vs Premium Account
- Free accounts come with 20 GB of base storage quota and transfer limits of 5 GB of per day.
- Premium account are from 400GB to 16TB.
- Business account from 3TB to 10PB.

## Data Extraction Methods
- Account takeover
- Online triage
- Data import
- Forensic tool

### Account takeover
- This method requires the Mega account to be handed over for evidence and further analysis or extraction.
- Also export the Recovery key, just in case.
- Issue of multi-factor authentication or accesses by other parties
- Pro
    -  Least effort among the methods
    -  No further change to the data by the user
    -  Issue of premium account: who to pay for the subscriptions
- Con
    - Data may be gone in the event, user attempt to reset the account
    - Contents may be removed by 3rd party or prohibited contents
    - Not suitable if account is not feasible 

1. On the target account, access 'My Files' or File Manager
2. Right click on the folder or file to be exported.
3. Click on 'Get Links'
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/mega003.png">
4. Copy the link generated
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/mega004.png">
5. Go to the forensic machine, use a web browser and create a Mega account

6. Create a folder with an identifier in the forensic machine Mega account
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/mega006.png">
7. Click on 'Import to my Cloud Drive' on the top-right corner, and import the date to the folder in Step 6.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/mega008.png">
8. You may still have transfer limit. In this case, subscribe to the preimum service to ocvercome the transfer limits.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/mega009.png">
9. Remove the links after the process is completed
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/mega010.png">

### Online triage
- This method is to log in to the Mega account, and to preview the contents manually
- Pro
    - Quick and easy for small dataset
    - Lesser legal requirements than Account takeover
- Con
    - Not suitable for large dataset 
    - Unreliable, may miss crucial evidence
    - Possibility of modifications and deletions

### Data import
- This method is to create a Mega account to import the data from the target's account
- Pro
    - Data synchronised instanteously, quickest way to secure data.
    - Lesser legal requirements
    - Overcome transfer limits by subscribing to a premium account to facilitate the data import
- Con
    - Legal consideration: essential creating a copy of the target data
    - Still require to extract the data for future analysis, verifications

### Forensic tool
- This method use the forensic tools available for data collection.
- Pro
    - Features to ensure data integrity - ensure data are stored in image container
    - Features may include data classification and data intelligence
- Con
    - Slow but steady to ensure data integrity
    - Avoid data throttle or transfer limits
    - Possibility of modification or deletion

## Forensic Tools

### Magnet Axiom Cloud/Cyber
<img width="300" alt="image" src="https://github.com/cisnerof/img/blob/main/mega012.png">
