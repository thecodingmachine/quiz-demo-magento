Quiz demo: Mouf + Magento
=========================

This repository contains a PHP Quiz demo application, running on Magento.

You can access the website by browsing http://demoquiz-magento.mouf-php.com

It is part of a wider demo, showcasing how to deploy on **same code** in many different environments.

The quiz code is stored in the [`thecodingmachine/quiz-module`](https://github.com/thecodingmachine/quiz-module) package.
It contains a [generic PSR-7 compatible controller](https://github.com/thecodingmachine/quiz-module/blob/master/src/Controllers/QuizController.php).
Using Mouf and a set of appropriate packages, the controller can then be deployed in a set of different environments:

- Mouf/Splash ([demo](http://demoquiz.mouf-php.com/)) ([code](https://github.com/thecodingmachine/quiz-demo-standalone))
- Wordpress ([demo](http://demoquiz-wordpress.mouf-php.com/)) ([code](https://github.com/thecodingmachine/quiz-demo-wordpress))
- Drupal 7 ([demo](http://demoquiz-drupal.mouf-php.com/)) ([code](https://github.com/thecodingmachine/quiz-demo-drupal))
- Joomla ([demo](http://demoquiz-joomla.mouf-php.com/)) ([code](https://github.com/thecodingmachine/quiz-demo-joomla))
- Magento ([demo](http://demoquiz-magento.mouf-php.com/)) ([code](https://github.com/thecodingmachine/quiz-demo-magento))

Installation
------------

- Clone the repository
- Run `composer install`
- Browse to the website root directory and run Magento install.
    - During install, enable the `Use Web Server (Apache) Rewrites` option.
- Copy the `.htaccess.sample` file to `.htaccess`
- Browse in the website and make sure the Apache rewrites are correctly set-up (you may need to tweek the .htaccess
  file and most notably the RewriteBase parameter).
- Browse to http://[your-website]/[path-to-magento]/vendor/mouf/mouf and run Mouf install process
- Connect to Magento administration http://[your-website]/[path-to-wordpress]/admin
- Purge your cache (System > Cache Management)
- You are done!
- Now, simply browse to: http://[your-website]/[path-to-magento]/quiz
