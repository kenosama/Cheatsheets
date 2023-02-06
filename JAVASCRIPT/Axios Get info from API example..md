```js
import axios from "axios";

const myFunction = async (parameterA, parameterB) => {

console.log('function starting?');



let apiUrl =

"https://api.openweathermap.org/geo/1.0/direct?q=" +

parameterA, +

"&limit=1&appid=" +

parameterB.key;

try {

const response = await axios.get(apiUrl);

console.log("response.data :>> ", response.data);

return response.data;

} catch (error) {

console.log("error :>> ", error);

}

};
	```
