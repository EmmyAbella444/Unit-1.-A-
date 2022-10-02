### QUIZ 001

| Input         | Output |
|---------------|--------|
| International | I11l   |
| My            | My     |
| Cat           | C1t    |
| (1b@!)        | (4)    |

### Solution to the Black Box

### Flowchart

### Code
String = input("Please enter a string: ")
lenght = int(len(String))

if lenght<3:   #Confirm that the string is bigger than 2 characteres
    print(String)

else:
    first = String[0] #First Character
    last = String[lenght-1] #Last Character
    middle = str(lenght-2) #Middle of string

print(f"{first}{middle}{last}")
