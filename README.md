# WestinPay Currency List Endpoint

WestinPay's Currency List Endpoint provides real-time exchange rates for over 152 currencies. To fetch the latest rates, use the endpoint below.

### Parameters

- **output**: Response output in either JSON or XML. Default: JSON.

## Code Examples

### cURL

<details>
  <summary>Code Example</summary>
  <pre><code>curl --location --request GET 'https://westinpay.com/currency/fiat_api?api_key=your_api_key&amp;output=JSON'</code></pre>
</details>

<details>
  <summary>Response</summary>
  <pre><code>{"valid":true,"currency_codes":["USD","AED","AFN","ALL","AMD","ANG","AOA","ZWL"]}</code></pre>
</details>

### PHP

<details>
  <summary>Code Example</summary>
  <pre><code>
// Your API key
$api_key = 'YOUR-API-KEY';
// API URL
$url = 'https://westinpay.com/currency/fiat_api?api_key=' . $api_key . '&output=JSON';
// Initialize cURL
$ch = curl_init();
// Set cURL options
curl_setopt($ch, CURLOPT_URL, $url);
curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
// Execute the cURL request
$response = curl_exec($ch);
// Close cURL
curl_close($ch);
// Print the response to the screen
echo $response;
  </code></pre>
</details>

<details>
  <summary>Response</summary>
  <pre><code>{"valid":true,"currency_codes":["USD","AED","AFN","ALL","AMD","ANG","AOA","ZWL"]}</code></pre>
</details>

### Node.js

<details>
  <summary>Code Example</summary>
  <pre><code>
const axios = require('axios');
const url = 'https://westinpay.com/currency/fiat_api?api_key=YOUR-API-KEY&output=JSON';
axios.get(url)
  .then(response => {
    console.log(response.data);
  })
  .catch(error => {
    console.error('Error fetching data:', error);
  });
  </code></pre>
</details>

<details>
  <summary>Response</summary>
  <pre><code>{"valid":true,"currency_codes":["USD","AED","AFN","ALL","AMD","ANG","AOA","ZWL"]}</code></pre>
</details>

<!-- Diğer diller için aynı yapıyı tekrarlayabilirsiniz -->

