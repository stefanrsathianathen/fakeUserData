# fakeUserData


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
### Generate Person
```
>>g.generatePerson()
{'id': 629943, 'firstName': 'Nairn', 'lastName': 'Maillard', 'email': 'NairnMaillard@qq.com', 'address': {'street': '2904 Warwick Lane', 'city': 'Kensington', 'state': 'NJ', 'zipCode': '71268'}, 'phoneNumber': '206-597-5325', 'birthday': {'month': 2, 'day': 25, 'year': 1998}, 'ssn': '171-71-1042', 'creditCardnumber': '341735124703280', 'password': 'IP2PPOgjtni'}
```

### Generate First Name
#### Takes in one optional parameter of gender from this list ['Male','Female','Other']
```
>>g.firstName()
'Tommye'
```
### Generate Last Name
```
>>g.lastName()
'Schuldt'
```

### Generate Email
#### Takes in three optional parameters: firstName (str), lastName(str), and length (int). The length is for the length of the email userName
```
>>g.email()
'JenifferMehtani@mac.com'
```

