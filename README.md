# Force.com Toolkit for PHP

The Force.com PHP Toolkit provides an easy-to-use wrapper for the Force.com Web Services SOAP API, presenting SOAP client implementations for both the enterprise and partner WSDLs.

See the [getting started guide](https://developer.salesforce.com/page/PHP_Toolkit_13.0_Getting_Started) for sample code to create, retrieve, update and delete records in the Force.com database.

## This specific packages notes

[![Latest Stable Version](https://img.shields.io/packagist/v/davispeixoto/force-dot-com-toolkit-for-php.svg)](https://packagist.org/packages/davispeixoto/force-dot-com-toolkit-for-php)
[![Total Downloads](https://img.shields.io/packagist/dt/davispeixoto/force-dot-com-toolkit-for-php.svg)](https://packagist.org/packages/davispeixoto/force-dot-com-toolkit-for-php)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/davispeixoto/Force.com-Toolkit-for-PHP/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/davispeixoto/Force.com-Toolkit-for-PHP/?branch=master)
[![Codacy Badge](https://www.codacy.com/project/badge/7c3e856c500046a882d061c09ed5aaca)](https://www.codacy.com/app/davis-peixoto/Force-com-Toolkit-for-PHP)
[![Code Climate](https://codeclimate.com/github/davispeixoto/Force.com-Toolkit-for-PHP/badges/gpa.svg)](https://codeclimate.com/github/davispeixoto/Force.com-Toolkit-for-PHP)
[![Build Status](https://travis-ci.org/davispeixoto/Force.com-Toolkit-for-PHP.svg?branch=master)](https://travis-ci.org/davispeixoto/Force.com-Toolkit-for-PHP)
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/eca47fa7-9ab3-431f-b551-217118408f1a/small.png)](https://insight.sensiolabs.com/projects/eca47fa7-9ab3-431f-b551-217118408f1a)

This fork is intended to make the Force.com Toolkit for PHP in packagist and will be used in my personal project to its classes and facilities available to be used in a Laravel 4 port.

The changes made by me (Davis Peixoto) are minor and won't change the core classes functionality, just make it available to be loaded by [composer](http://getcomposer.org/).

Once the main project by [developerforce](https://gitub.com/developerforce/) is available though composer, this fork can be dropped and replaced by the original.

About the fixes:
- I've just removed all unused code from composer point of view. I've ported all classes into src folder, and kept all of them into a separated file (there was some files with multiple classes).
- I've formatted code into PSR-1/PSR-2 format
- I've changed some methods signatures, changing their type, like from **date** to **string**, in order to give them the proper type according to current usage. I've not added/removed parameters from phpdoc signatures, despite the high amount of errors.
