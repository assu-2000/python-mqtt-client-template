# python-mqtt-client-template as part of AsyncAPI/GSoC Apk 2024
Creating a template


This tutorial teaches  how to create a simple generator template using a Python MQTT client. You'll use the AsyncAPI document and the template you develop to generate Python code. Additionally, you'll create template code with a reusable component to reuse the custom functionality you create and test your code using an MQTT client.

Suppose you can only sleep when the AC in your bedroom is set to 22 °C, and you can't sleep when the temperature drops or rises above that. You can install a smart monitor in your bedroom that keeps track of the temperature and notifies you to adjust it to your optimum temperature when it fluctuates. You will create a template to alert you when the bedroom's temperature fluctuates from 22 °C.

In this tutorial:

You'll use the Eclipse Mosquito MQTT broker, which you'll connect to subscribe and publish messages using an MQTT client.
You'll use Python Paho-MQTT as the MQTT client in this project.
You'll create a React template that will use the MQTT broker to allow you to monitor your bedroom's temperature and notify you when the temperature drops or rises above 22 °C.
Lastly, create a reusable component for the output code's sendTemperatureDrop and sendTemperatureRise functions.
Background context
There is a list of community maintained templates, but what if you do not find what you need? In that case, you'll create a user-defined template that generates custom output from the generator. Before you create the template, you'll need to have an AsyncAPI document that defines the properties you want to use in your template to test against. In this tutorial, you'll use the following template saved in the test/fixtures/asyncapi.yml file in your template project directory.