# Unit-1.-A-
# Crypto Wallet

# Criteria A: Planning

## Problem definition

My client is Ms. Jones. She just moved in to live alone and needs to organize her expenses. She has a lot of interest in cryptocurrencies and currently she is using spreadsheets to store her entire expenses database and so has been facing difficulties in keeping all the data organized because it is not possible for her to find useful statistics of her expenses, and she’s having trouble getting organized with the transactions.

HER DATABASE

FOOD...........02/09/2022.....100 DOT
RENT...........03/09/2022.....500 DOT
TRAVEL.........04/09/2022.....600 DOT
FOOD...........05/10/2022.....900 DOT
SAVING.........06/10/2022.....4000 DOT
TRAVEL.........07/10/2022.....2000 DOT
FOOD............02/11/22......1000 DOT
FOOD...........06/11/2022.....200 DOT
FOOD...........03/11/2022.....300 DOT
RENT...........09/12/2022.....500 DOT
SAVING.........10/10/2022.....6000 DOT
FOOD...........03/08/2022.....200 DOT
FOOD...........01/10/2022.....50 DOT
FOOD...........12/10/2022.....300 DOT
FOOD...........12/09/2022.....100 DOT
TRAVEL.........10/09/2022.....100 DOT
FOOD...........09/10/2022.....200 DOT
RENT...........09/10/2022.....500 DOT


## Proposed Solution

Design statement:
I will to design and make a Digial Wallet for a client who is Ms. Jones. The Digital wallet will about ———— and is constructed using the software pyvharm. It will take  ———- to make and will be evaluated according to the criteria ———.


## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4. The eletronic ledger show all data organized
5. The eletronic Ledger show grap of  transactions
6. the eletronic Ledger show useful informations of Polkadot
7. The eletronic Ledger show the total spend, the total spend by category and by month.
8. The eletronic ledger can convert Polkadot to Dollars
9. The eletronic Ledger can show informations about the program and author
10. The eletronic Ledger ca show the total amount saved.
11. The eletronic Ledge can allow the user to sign in and create a new account or to just login.
12. The eletronic Ledger has a safe login system to protect the data
13. the system has different functions to validate the input

# Criteria B: Design

## System Diagram!

![Screen Shot 2022-10-09 at 1 25 53](https://user-images.githubusercontent.com/111819437/194717569-5c5c2e9a-099d-4881-bdf0-83658332774e.png)




## Flow Diagrams


## Record of Tasks
| Task No | Planned Action                                                | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Create system diagram                                         | To have a clear idea of the hardware and software requirements for the proposed solution                        | 10min         | Sep 24                 | B         |

# Criteria C: Development
## Video
https://drive.google.com/file/d/1xSMWb3NAR36VVdIT2tJIxBc5eABkqSQU/view?usp=sharing

## Login System
My client requires a system to protect the private data. I thought about using a login system to accomplish this requirement using a if condition and the open command to work with a csv file. More description of the code....
```.py
def simple_login(user:str, password:str)->bool:
    '''
    Simple authentication, needs fle user.csv
    :param user: string
    :param password: string
    :return: True/False if user is in database
    '''
    with open("user.csv") as file:
        database = file.readlines()
    output = False
    for line in database:
        line_cleaned = line.strip() #remove \n
        user_pass = line_cleaned.split(",")
        if user == user_pass[0] and password == user_pass[1]:
            output = True
            break

    return output


```
