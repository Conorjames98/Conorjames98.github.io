+++
date = '2025-01-05T21:55:19Z'
draft = false
title = 'API Staus Check'
+++

# A simple application to check the staus  of various APIs 


I have created a small application in python that allows the user to enter the url of the api endpoint to check the status of the API the application could be expanded on for POST requests to the api for the creation of long-life-tokens which would be needed for further interaction with the API.


```py
import requests

def check_api():
    while True:
        # GET the API url from the user
        url = input("Enter the API URL you want to check: ").strip()

        #A header section for any necessary headers
        #A token or key (will be needed in the expansion 

        #of the program once a bearer token is aquired)
        headers = {
            "Authorization": "Bearer your_api_key",
            "Content-Type": "application/json"
        }
 
        # Make the GET request
        try:
            response = requests.get(url, headers=headers)

            # Check the status of the the API
            if response.status_code == 200:
                print("API is nominal!")
                print("Response:", response.json())
            else:
                print(f"API health check failed with status code: {response.status_code}")
                print("Response:", response.text)

        except requests.exceptions.RequestException as e:
            print(f"An error occurred: {e}")

        # Allows the user to check another API
        another = input("Would you like to check another API? (yes/no): ").strip().lower()
        if another != 'yes':
            print("Goodbye!")
            break

# Runs the function again if condition is met
check_api()

```