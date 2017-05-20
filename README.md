# fakeUserData
#### A python package that generates fake user data for testing purposes

## Installation
```
pip install fakeUserData
```

## Usage
```
from fakeUserData import generator 
```
## Better Use (What is used in the following examples)
```
from fakeUserData import generator as g
```
### Person
```
>>g.generatePerson()
{'id': 629943, 'firstName': 'Nairn', 'lastName': 'Maillard', 'email': 'NairnMaillard@qq.com', 'address': {'street': '2904 Warwick Lane', 'city': 'Kensington', 'state': 'NJ', 'zipCode': '71268'}, 'phoneNumber': '206-597-5325', 'birthday': {'month': 2, 'day': 25, 'year': 1998}, 'ssn': '171-71-1042', 'creditCardnumber': '341735124703280', 'password': 'IP2PPOgjtni'}
```

### First Name
#### Takes in one optional parameter of gender from this list ['Male','Female','Other']
```
>>>g.firstName()
'Tommye'
>>>g.firstName('Female')
'Rosalina'
```
### Last Name
```
>>>g.lastName()
'Schuldt'
```

### Email
#### Takes in three optional parameters: firstName (str), lastName(str), and length (int). The length is for the length of the email userName
```
>>>g.email()
'JenifferMehtani@mac.com'
>>>g.email(g.firstName(),g.lastName(),15)
'DonaldRazey1QCPy@orange.fr'
```
### Birthday
###  Returns a tuple in format (day,month,year).
```
>>>g.birthday()
(29, 11, 1994)
```

### Country
```
>>> g.Country()
'Sri Lanka'
```
### Social Security Number
```
>>> g.ssn()
'362-04-9527'
```
### Password
#### Takes in one optional argument of length to specify the lenght of the password
```
>>> g.createPassword()
'E@jQDG!s((y'
>>> g.createPassword(24)
'Z=8g^yKX92ZUC8Gy!Gf_q36%9'
```
### Creditcard 
#### Takes in one optional parameter of card brand from this list ['Amex','MasterCard','Visa']
```
>>> g.creditCard()
'4532500517930'
>>> g.creditCard('Amex')
'375259649382900'
```
### US Address 
```
>>> g.usAddress()
('5037 Prescott Lane', 'Seekonk', 'HI', '38510')
```
### Street Name
```
>>> g.street()
'9721 Park Avenue'
```
### US city name
```
>>> g.city()
'Hancock'
```
### US state (Short Form Only)
```
>>> g.state()
'LA'
```
### US zipCode
```
>>> g.zipCode()
'22287'
```
### random Date
#### Follows same return format as birthday
```
>>> g.randomDate()
(6, 12, 1928)
```
### id Number
### Takes one optional parameter of length of the id number
```
>>> g.id()
324200
>>> g.id(12)
82892460937
```
### IP Address 
```
>>> g.ipAddress()
'199.67.822.241'
```
### UserName
#### Takes one optional parameter of length of the user number
```
>>> g.userName()
'LitrellN'
>>> g.userName(10)
'JJ5a7G7hVb'
```
### US Phone Number
#### Takes one optional parameter of area code
```
>>> g.usPhoneNumber()
'420-584-3523'
>>> g.usPhoneNumber(510)
'510-955-8706'
```
