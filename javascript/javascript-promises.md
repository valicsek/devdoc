# Javascript Promises

## Read a file with promise using fs (Node.JS)

This example shows how can you read a file like `myfile.json` using Node.JS with Promise.

```javascript
const fs = require('fs')

function readWithPromise(file_name) 
{
    return new Promise((resolve, reject) => 
	{
        fs.readFile(file_name, 'utf8', (err, data) => 
		{
            if (err) reject(err)
            resolve(data);
        });
    });
}

// Example usage of this Promise
readWithPromise('myfile.json')
    .then((fileContext) => 
    {
    	console.log(fileContext)
	})
```

