# Frig Studio

This document is the documentation for the grifon API.


### GET parameters

#### pretty

The pretty parameter is set to true by default and is used to specify the format of the json output. The valid values are :

- 0
- 1
- false
- true

Here is a request with the pretty parameter set to **true**

```
	GET https://frigstudio.com/grifon/users/1?pretty=true
```

```javascript
	{
      "id": "1",
      "name": "Alexandre Frigon"
    }
```

Here is a request with the pretty parameter set to **false**

```
	GET https://frigstudio.com/grifon/users/1?pretty=false
```

```javascript
	{"id": "1","name": "Alexandre Frigon"}
```

### Error codes

Code | description
---- | -----------
0001 | Page not found
1000 | Bad GET field
1001 | Bad GET value
1003 | Bad GET parameters
