# Unit-1.-A-
# Crypto Wallet

# Criteria A: Planning

## Problem definition

My client is Ms. Jones. She just moved in to live alone and needs to organize her expenses. She has a lot of interest in cryptocurrencies and currently she is using spreadsheets to store her entire expense database and so has been facing difficulties in keeping all the data organized because it is not possible for her to find useful statistics of her expenses, and she’s having trouble getting organized with the transactions.

DATABASE

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

| Date | Description | Category | Amount  |
|------|-------------|----------|---------|
| Sep 23 2022 | bought a house | Expenses | 10 BTC |
| Sep 24 2022 | food for house celebration | Food | 0.000001 BTC |


## Proposed Solution

Design statement:
I will to design and make a ———— for a client who is ———. The ——– will about ———— and is constructed using the software ———. It will take  ———- to make and will be evaluated according to the criteria ———.

** add a description of your coin and citation **
| Group 1   |              |   | Group  2  |           |
|-----------|--------------|---|-----------|-----------|
| Developer | Digital Coin |   | Developer | Coin      |
| Alex      | Bitcoin      |   | Alek      | Solana    |
| Bernard   | Ethereum     |   | Mai       | Dogecoin  |
| Yutaro    | Dogecoin     |   | Daniela   | BInance   |
| Verlon    | Apecoin      |   | Kris      | Bitcoin   |
| Oswell    | Tether       |   | Paula     | Lumens    |
| Thumula   | Tron         |   | ZAven     | Ethereum  |
| Ainee     | Mana         |   | Jonathan  | Maker     |
| Lison     | Solana       |   | Kai       | Avalanche |
| Sabu      | Binance      |   | Daiichiro | Flow      |
| Emmy      | Polkadot     |   | Masamu    | Cardano   |
| Maria     | Cardano      |   | Yasmina   | Zcash     |
| Zelan     | Cosmos       |   | Jana      | LiteCoin  |
| Manahil   | BinanceUSD   |   | Lyn       | Iota      |
| Krish     | UsdCoin      |   | Meisa     | Polkadot  |
|           |              |   | Mayte     | Cosmos    |
|           |              |   | Pop       | Ripple    |
Justify the tools/structure of your solution

## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4.
5.
6.

# Criteria B: Design

## System Diagram!
[Screen Shot 2022-10-04 at 10 26 26](https://user-images.githubusercontent.com/111819437/194717407-6111f888-07ae-4b4d-bbfc-a760cdf2e316.png)



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
