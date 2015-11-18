Quiz demo: Mouf + Magento
=========================

This repository contains a PHP Quiz demo application, running on Magento.

You can access the website by browsing http://demoquiz-magento.mouf-php.com

It is part of a wider demo, showcasing how to deploy on **same code** in many different environments.

Installation
------------

- Clone the repository
- Run `composer install`
- Browse to the website root directory and run Magento install.
    - During install, enable the `Use Web Server (Apache) Rewrites` option.
- Browse to http://[your-website]/[path-to-magento]/vendor/mouf/mouf and run Mouf install process
- Connect to Magento administration http://[your-website]/[path-to-wordpress]/admin
- Purge your cache (System > Cache Management)
- You are done!
- Now, simply browse to: http://[your-website]/[path-to-magento]/quiz
