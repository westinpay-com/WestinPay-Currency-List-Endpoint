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


| Country                       | Currency                       | ISO Code |
|-------------------------------|--------------------------------|----------|
| United States Dollar          | United States Dollar           | USD      |
| United Arab Emirates Dirham   | United Arab Emirates Dirham    | AED      |
| Afghan Afghani                | Afghan Afghani                 | AFN      |
| Albanian Lek                  | Albanian Lek                   | ALL      |
| Armenian Dram                 | Armenian Dram                  | AMD      |
| Netherlands Antillean Guilder | Netherlands Antillean Guilder  | ANG      |
| Angolan Kwanza                | Angolan Kwanza                 | AOA      |
| Argentine Peso                | Argentine Peso                 | ARS      |
| Australian Dollar             | Australian Dollar              | AUD      |
| Aruban Florin                 | Aruban Florin                  | AWG      |
| Azerbaijani Manat             | Azerbaijani Manat              | AZN      |
| Bosnia-Herzegovina Convertible Mark | Bosnia-Herzegovina Convertible Mark | BAM  |
| Barbadian Dollar              | Barbadian Dollar               | BBD      |
| Bangladeshi Taka              | Bangladeshi Taka               | BDT      |
| Bulgarian Lev                 | Bulgarian Lev                  | BGN      |
| Bahraini Dinar                | Bahraini Dinar                 | BHD      |
| Burundian Franc               | Burundian Franc                | BIF      |
| Bermudian Dollar              | Bermudian Dollar               | BMD      |
| Brunei Dollar                 | Brunei Dollar                  | BND      |
| Bolivian Boliviano            | Bolivian Boliviano             | BOB      |
| Brazilian Real                | Brazilian Real                 | BRL      |
| Bahamian Dollar               | Bahamian Dollar                | BSD      |
| Bhutanese Ngultrum            | Bhutanese Ngultrum             | BTN      |
| Botswana Pula                 | Botswana Pula                  | BWP      |
| Belarusian Ruble              | Belarusian Ruble               | BYN      |
| Belize Dollar                 | Belize Dollar                  | BZD      |
| Canadian Dollar               | Canadian Dollar                | CAD      |
| Congolese Franc               | Congolese Franc                | CDF      |
| Swiss Franc                   | Swiss Franc                    | CHF      |
| Chilean Peso                  | Chilean Peso                   | CLP      |
| Chinese Yuan                  | Chinese Yuan                   | CNY      |
| Colombian Peso                | Colombian Peso                 | COP      |
| Costa Rican Colón             | Costa Rican Colón              | CRC      |
| Cuban Peso                    | Cuban Peso                     | CUP      |
| Cape Verdean Escudo           | Cape Verdean Escudo            | CVE      |
| Czech Koruna                  | Czech Koruna                   | CZK      |
| Djiboutian Franc              | Djiboutian Franc               | DJF      |
| Danish Krone                  | Danish Krone                   | DKK      |
| Dominican Peso                | Dominican Peso                 | DOP      |
| Algerian Dinar                | Algerian Dinar                 | DZD      |
| Egyptian Pound                | Egyptian Pound                 | EGP      |
| Eritrean Nakfa                | Eritrean Nakfa                 | ERN      |
| Ethiopian Birr                | Ethiopian Birr                 | ETB      |
| Euro                          | Euro                           | EUR      |
| Fijian Dollar                 | Fijian Dollar                  | FJD      |
| Falkland Islands Pound        | Falkland Islands Pound         | FKP      |
| Faroese Króna                 | Faroese Króna                  | FOK      |
| British Pound Sterling        | British Pound Sterling         | GBP      |
| Georgian Lari                 | Georgian Lari                  | GEL      |
| Guernsey Pound                | Guernsey Pound                 | GGP      |
| Ghanaian Cedi                 | Ghanaian Cedi                  | GHS      |
| Gibraltar Pound               | Gibraltar Pound                | GIP      |
| Gambian Dalasi                | Gambian Dalasi                 | GMD      |
| Guinean Franc                 | Guinean Franc                  | GNF      |
| Guatemalan Quetzal            | Guatemalan Quetzal             | GTQ      |
| Guyanaese Dollar              | Guyanaese Dollar               | GYD      |
| Hong Kong Dollar              | Hong Kong Dollar               | HKD      |
| Honduran Lempira              | Honduran Lempira               | HNL      |
| Croatian Kuna                 | Croatian Kuna                  | HRK      |
| Haitian Gourde                | Haitian Gourde                 | HTG      |
| Hungarian Forint              | Hungarian Forint               | HUF      |
| Indonesian Rupiah             | Indonesian Rupiah              | IDR      |
| Israeli New Shekel            | Israeli New Shekel             | ILS      |
| Manx pound                    | Manx pound                     | IMP      |
| Indian Rupee                  | Indian Rupee                   | INR      |
| Iraqi Dinar                   | Iraqi Dinar                    | IQD      |
| Iranian Rial                  | Iranian Rial                   | IRR      |
| Icelandic Króna               | Icelandic Króna                | ISK      |
| Jersey Pound                  | Jersey Pound                   | JEP      |
| Jamaican Dollar               | Jamaican Dollar                | JMD      |
| Jordanian Dinar               | Jordanian Dinar                | JOD      |
| Japanese Yen                  | Japanese Yen                   | JPY      |
| Kenyan Shilling               | Kenyan Shilling                | KES      |
| Kyrgyzstani Som               | Kyrgyzstani Som                | KGS      |
| Cambodian Riel                | Cambodian Riel                 | KHR      |
| Kiribati Dollar               | Kiribati Dollar                | KID      |
| Comorian Franc                | Comorian Franc                 | KMF      |
| South Korean Won              | South Korean Won               | KRW      |
| Kuwaiti Dinar                 | Kuwaiti Dinar                  | KWD      |
| Cayman Islands Dollar         | Cayman Islands Dollar          | KYD      |
| Kazakhstani Tenge             | Kazakhstani Tenge              | KZT      |
| Laotian Kip                   | Laotian Kip                    | LAK      |
| Lebanese Pound                | Lebanese Pound                 | LBP      |
| Sri Lankan Rupee              | Sri Lankan Rupee               | LKR      |
| Liberian Dollar               | Liberian Dollar                | LRD      |
| Lesotho Loti                  | Lesotho Loti                   | LSL      |
| Libyan Dinar                  | Libyan Dinar                   | LYD      |
| Moroccan Dirham               | Moroccan Dirham                | MAD      |
| Moldovan Leu                  | Moldovan Leu                   | MDL      |
| Malagasy Ariary               | Malagasy Ariary                | MGA      |
| Macedonian Denar              | Macedonian Denar               | MKD      |
| Myanmar Kyat                  | Myanmar Kyat                   | MMK      |
| Mongolian Tugrik              | Mongolian Tugrik               | MNT      |
| Macanese Pataca               | Macanese Pataca                | MOP      |
| Mauritanian Ouguiya           | Mauritanian Ouguiya            | MRU      |
| Mauritian Rupee               | Mauritian Rupee                | MUR      |
| Maldivian Rufiyaa             | Maldivian Rufiyaa              | MVR      |
| Malawian Kwacha               | Malawian Kwacha                | MWK      |
| Mexican Peso                  | Mexican Peso                   | MXN      |
| Malaysian Ringgit             | Malaysian Ringgit              | MYR      |
| Mozambican Metical            | Mozambican Metical             | MZN      |
| Namibian Dollar               | Namibian Dollar                | NAD      |
| Nigerian Naira                | Nigerian Naira                 | NGN      |
| Nicaraguan Córdoba            | Nicaraguan Córdoba             | NIO      |
| Norwegian Krone               | Norwegian Krone                | NOK      |
| Nepalese Rupee                | Nepalese Rupee                 | NPR      |
| New Zealand Dollar            | New Zealand Dollar             | NZD      |
| Omani Rial                    | Omani Rial                     | OMR      |
| Panamanian Balboa             | Panamanian Balboa              | PAB      |
| Peruvian Nuevo Sol            | Peruvian Nuevo Sol             | PEN      |
| Papua New Guinean Kina        | Papua New Guinean Kina         | PGK      |
| Philippine Peso               | Philippine Peso                | PHP      |
| Pakistani Rupee               | Pakistani Rupee                | PKR      |
| Polish Zloty                  | Polish Zloty                   | PLN      |
| Paraguayan Guarani            | Paraguayan Guarani             | PYG      |
| Qatari Riyal                  | Qatari Riyal                   | QAR      |
| Romanian Leu                  | Romanian Leu                   | RON      |
| Serbian Dinar                 | Serbian Dinar                  | RSD      |
| Russian Ruble                 | Russian Ruble                  | RUB      |
| Rwandan Franc                 | Rwandan Franc                  | RWF      |
| Saudi Riyal                   | Saudi Riyal                    | SAR      |
| Solomon Islands Dollar        | Solomon Islands Dollar         | SBD      |
| Seychellois Rupee             | Seychellois Rupee              | SCR      |
| Sudanese Pound                | Sudanese Pound                 | SDG      |
| Swedish Krona                 | Swedish Krona                  | SEK      |
| Singapore Dollar              | Singapore Dollar               | SGD      |
| Saint Helena Pound            | Saint Helena Pound             | SHP      |
| Sierra Leonean Leone          | Sierra Leonean Leone           | SLL      |
| Somali Shilling               | Somali Shilling                | SOS      |
| Surinamese Dollar             | Surinamese Dollar              | SRD      |
| South Sudanese Pound          | South Sudanese Pound           | SSP      |
| São Tomé and Príncipe Dobra   | São Tomé and Príncipe Dobra    | STN      |
| Syrian Pound                  | Syrian Pound                   | SYP      |
| Swazi Lilangeni               | Swazi Lilangeni                | SZL      |
| Thai Baht                     | Thai Baht                      | THB      |
| Tajikistani Somoni            | Tajikistani Somoni             | TJS      |
| Turkmenistani Manat           | Turkmenistani Manat            | TMT      |
| Tunisian Dinar                | Tunisian Dinar                 | TND      |
| Tongan Pa'anga                | Tongan Pa'anga                 | TOP      |
| Turkish Lira                  | Turkish Lira                   | TRY      |
| Trinidad and Tobago Dollar    | Trinidad and Tobago Dollar     | TTD      |
| Tuvaluan Dollar               | Tuvaluan Dollar                | TVD      |
| New Taiwan Dollar             | New Taiwan Dollar              | TWD      |
| Tanzanian Shilling            | Tanzanian Shilling             | TZS      |
| Ukrainian Hryvnia             | Ukrainian Hryvnia              | UAH      |
| Ugandan Shilling              | Ugandan Shilling               | UGX      |
| Uruguayan Peso                | Uruguayan Peso                 | UYU      |
| Uzbekistan Som                | Uzbekistan Som                 | UZS      |
| Venezuelan Bolívar            | Venezuelan Bolívar             | VES      |
| Vietnamese Dong               | Vietnamese Dong                | VND      |
| Vanuatu Vatu                  | Vanuatu Vatu                   | VUV      |
| Samoan Tala                   | Samoan Tala                    | WST      |
| Central African CFA Franc     | Central African CFA Franc      | XAF      |
| East Caribbean Dollar         | East Caribbean Dollar          | XCD      |
| Special Drawing Rights        | Special Drawing Rights         | XDR      |
| West African CFA Franc        | West African CFA Franc         | XOF      |
| CFP Franc                     | CFP Franc                      | XPF      |
| Yemeni Rial                   | Yemeni Rial                    | YER      |
| South African Rand            | South African Rand             | ZAR      |
| Zambian Kwacha                | Zambian Kwacha                 | ZMW      |
| Zimbabwean Dollar             | Zimbabwean Dollar              | ZWL      |


<!-- Diğer diller için aynı yapıyı tekrarlayabilirsiniz -->

