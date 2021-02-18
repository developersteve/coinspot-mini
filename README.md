Mini SDK for the read only coinspot API, this only contains what you need to get account balances and transactions.

Have a look at https://www.coinspot.com.au/api for more info on the CoinSpot API.

Example usage

```javascript
var coinspot = require('coinspot-mini');

var secret = ''; // insert your secret here
var key = ''; // insert your key here

var client = new coinspot(key, secret);

client.balances(function(e, data) {
 	console.log(data);
}); 

client.transactions(function(e, data) {
 	console.log(data);
});


```