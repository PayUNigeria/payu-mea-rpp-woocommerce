# payu-mea-rpp-woocommerce

## Installation (WooCommerce) 

### 1. Install Wordpress and WooCommerce
Wordpress is free web software you can use to create an online website. The core software is built by hundreds of community volunteers with thousands of plugins and themes available to transform your site into almost anything you can imagine. Visit Wordpress website for more information: http://www.wordpress.org/

WooCommerce is a free bolt-on shopping cart that lets customers buy your products, services and digital downloads online. Visit WooCommerce website for more information: http://www.woothemes.com/woocommerce/

### 2. Download the PayU/WooCommerce plugin and upload to Wordpress installation
Download the PayU/WooCommerce plugin from the github repository: https://github.com/PayUNigeria/payu-mea-rpp-woocommerce and unzip the downloaded file - it should contain a folder named payuMeaRppWooCommerce.
Upload the payuMeaRppWooCommerce folder to the wordpress plugins directory - <wordpress webroot>/wp-content/plugins

### 3. WooCommerce Payment Gateway Setup
Login to the Wordpress administration interface

![1](https://cloud.githubusercontent.com/assets/4561020/16078404/ac22fa16-32f6-11e6-85c3-f08825cdeaf2.jpg)

Once logged in, select Plugins > WooCommerce from the main administration menu to the left of the page and activate the WooCommerce plugin, if not already activated.
Next select Plugins > WooCommerce PayU RPP from the main administration menu to the left of the page and activate the WooCommerce PayU RPP plugin.

![2](https://cloud.githubusercontent.com/assets/4561020/16078430/df078b4a-32f6-11e6-9d2e-9d9bb68a5066.jpg)

The WooCommerce menu item will now be available from the main administration menu. You can configure and activate the PayU MEA plugin by selecting: #### Settings > Payment Gateways > PayU MEA.

![3](https://cloud.githubusercontent.com/assets/4561020/16078469/0e7373ee-32f7-11e6-9164-526e3fe6b030.jpg)

Update the configuration (options described below) by clicking on the **Save changes** button.

![4](https://cloud.githubusercontent.com/assets/4561020/16078484/28048578-32f7-11e6-9a8c-e5af025ae25d.jpg)

#### Configuration form options:

| **Configuration Option**        | **Description**           |
| -------------                   |-------------            |
| Enable/Disable                  | Determines if PayU should be available as a payment option on the front-end (checkbox ticked = yes/active) |
| Title                           | What should be displayed on the fron-tend to the customer making a payment e.g. PayU MEA      |
| Description                     | What should be displayed on the front-end to the customer making a payment e.g. Credit Card (Processed by PayU)      |
| SafeKey                         | SafeKey in {XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX} format: (Production value is provided by PayU, Staging value is entered already and can't be updated)      |
| Username                        | SOAP API Username used in transactions (Production value is provided by PayU, Staging value is entered already and can't be updated)      |
| Password                        | SOAP API Password used in transactions (Production value is provided by PayU, Staging value is entered already and can't be updated)      |
| Currency                        | The currency used for transactions (Only the 'NGN' currency is currently supported in this plugin/extension and value cannot be altered)      |
| Payment method                  | Payment method(s) used for transactions      |
| Payment Type                  | Transaction type used for transactions (Only the 'PAYMENT' transaction type is currently supported in this plugin/extension and value should not be altered)      |
| PayU sandbox                  | Checkbox indicating which PayU environment to use for transactions (Staging: used testing and integration, Production: used for live/real transactions)      |
| Payment Notification Email Addresses                  | Email address where payment notifications statuses will be sent      |
