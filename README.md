# Unit-1.-A-
# Crypto Wallet

![](22ROOSE-master768.gif)  
<sub>Illustration for Glenn Harvey</sub>

# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all his transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. 

Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.

An example of the data stored is 

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
