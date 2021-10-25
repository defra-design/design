# Defra page template for internal services

A defra page template for internal services [which are not on GOV.UK](https://www.gov.uk/service-manual/design/making-your-service-look-like-govuk#if-your-service-isnt-on-govuk).

## Add to your Project
Install in the kit

'''
npm install cathydutton/layout-defra
'''

Replace this line

'''
{% extends "layout.html" %}
'''

With...

'''
{% extends 'layout-defra.html' %}
'''

Just above the layout include set the service name...

'''
{% set DefraServiceName = "My service name" %}
'''
