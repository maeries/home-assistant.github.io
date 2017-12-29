---
layout: page
title: "Installation in Python virtual environment"
description: "How to install Home Assistant in a Python virtual environment."
date: 2016-4-16 16:40
sidebar: true
comments: false
sharing: true
footer: true
redirect_from: /getting-started/installation-virtualenv/
---

If you already have Python 3.5 or later installed, you can easily give Home Assistant a spin.

It's recommended when installing Python packages that you use a [virtual environment](https://docs.python.org/3.5/library/venv.html#module-venv). This will make sure that your Python installation and Home Assistant installation won't impact one another. The following steps will work on most unix like systems.

_(If you're on a Debian based system, you will need to install Python virtual environment support using `apt-get install python3-pip python3-venv`.)_

### {% linkable_title Install %}

 1. Create a virtual environment in your current directory:
    ```
    $ python3 -m venv homeassistant
    ```
 2. Open the virtual environment:
    ```
    $ cd homeassistant
    ```
 3. Activate the virtual environment:
    ```
    $ source bin/activate
    ```
 4. Install Home Assistant:
    ```
    $ python3 -m pip install homeassistant
    ```
 5. Configure it to [autostart](docs/autostart/)
 6. Or run Home Assistant manually:
    ```
    $ hass --open-ui
    ```
 
### {% linkable_title Upgrade %}

 1. Stop Home Assistant

 2. Open the directory where the virtual environment is located:
    ```
    $ cd homeassistant
    ```
 3. Activate the virtual environment:
    ```
    $ source bin/activate
    ```
 4. Upgrade Home Assistant:
    ```
    $ python3 -m pip install --upgrade homeassistant
    ```
 5. Start Home Assistant

### {% linkable_title Notes %}

- In the future, if you want to start Home Assistant manually again, follow step 2, 3 and 5.
- It's recommanded to run Home Assistant as a dedicated user.

<p class='info'>
Looking for more advanced guides? Check our [Rasbian guide](/docs/installation/raspberry-pi/) or the [other installation guides](docs/installation)
</p>
