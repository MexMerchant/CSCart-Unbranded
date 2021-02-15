# README

# Contents

- Introduction
- Prerequisites
- Rebranding
- Installing and configuring the module
- License

# Introduction

This CS Cart module provides an easy method to integrate with the payment gateway.
 - The httpdocs directory contains the files that need to be uploaded to the root directory of where CS Cart is installed
 - Supports CS Cart versions: **4.x+**

# Prerequisites

- The module requires the following prerequisites to be met in order to function correctly:
    - For a full list of requirements please see: https://docs.cs-cart.com/latest/install/system_requirements.html
    - SSL **NB: HTTPS is expected to be in place as the payment gateway will respond over SSL when integrating directly. Failure to provide an environment where HTTPS traffic is possible, will result in the 3DSv2 payment flow failing***

> Please note that we can only offer support for the Module itself. While every effort has been made to ensure the payment module is complete and bug free, we cannot guarentee normal functionality if unsupported changes are made.

# Rebranding

To rebrand this module, complete the following steps:

1. In file `httpdocs/app/addons/payment_network/addon.xml` change the following:
	- Line 3: `<id>payment_network</id>` change Payment Network to your brand name
	- Line 4: `<name>Payment Network</name>` change Payment Network to your brand name
2. In file `httpdocs/app/addons/payment_network/config.php` change the following:
	- Line 5: change the URL to that which we supply
	- Line 6: change the URL to that which we supply
	- Line 7: change the URL to that which we supply
	- Line 14: change the ID to that which we supply
	- Line 15: change the SECRET to that which we supply

# Installing and configuring the module

1. Unzip / untar and merge the httpdocs folder into the root folder of your CS-Cart installation.
2. Login to your CS-Cart installation and navigate to Administration > Payment Methods from the top menu
3. Click the '+' symbol at the top of the page to add a new payment method.
4. Fill out the form and select Cardstream as the processor. Click on the 'Configure' tab and enter the relevant information before clicking 'Create'.
5. The module will now be available as a payment method in the checkout procedure.

License
----
MIT
