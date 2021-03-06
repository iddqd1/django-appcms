# django-appcms
Django-AppCMS is a extention for django-cms that adds templatetags for inserting django-cms placeholders in app templates. It enables front end editing of content in your apps.

## Requirements
Since version 0.0.13:
django-cms >= 3.1

## Installation
Django-AppCMS can be installed with pip:

	pip install django-appcms

## Usage
- Add appcms to INSTALLED\_APPS in your settings.py file:

		INSTALLED_APPS = (
			...
			'appcms',
			...
		)

- Run ./manage.py syncdb to add tables for django-appcms

- Load appcms\_tags in your template:

		{% load appcms_tags %}

- Add a placeholder:

		{% appcms_placeholder "name_of_placeholder" %}

- Make sure the base template includes the django-cms toolbar

When the view loads with a admin logged in editing can be enabled in the django-toolbar.
