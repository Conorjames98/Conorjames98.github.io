+++
date = '2025-01-05T22:46:51Z'
draft = false
title = 'Virtual Enviroments (Python)'
+++


# How to start a virtual enviroment for python on MAC/Windows

A simple but necessary feature of python to stop package conflicts with globbaly installed packages, I had used this feature to make sure when I was installing packages very specific to the project I was working on that I did not install them globablly and caused myself more issues.
 

## On Mac OS

  1. Make sure Python is correctly installed

  2. On your favourite IDE open the terminal and type

```bash
python3 -m venv myenv
```
3. Then activate the virtual enviroment with 

```bash
source myenv/bin/activate
```

## On Windows

```bash
python -m venv venv
```
Activate the virtual enviroment with

```bash
myenv\Scripts\activate
```
