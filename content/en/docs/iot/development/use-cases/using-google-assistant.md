---
title: Using Google Assistant
date: 2020-03-18
weight: 20
toc: true
---

In w
        }
    }
    {
        "provider": "googleassistant",
        "response": {
            "partial": "what's the weather"
        }
    }

    # Then Google Assistant returns the response to your question.
    # If you have a speaker, you can hear the response.
    {
        "provider":"googleassistant",
        "response":{
            "displayText":"Looks kind of cloudy Right now in Seoul it's 51 and mostly cloudy. Today, it'll be partly cloudy, with a forecasted high of 51 and a low of 32.
            ---
            ( More on weather.com )"
        }
    }

    # Press Ctrl+C to quit the getResponse method
    ```

4. To stop the service, call `stop` method:

    ``` shell
    root@raspberrypi4:/sysroot/home/root# luna-send -n 1 -f luna://com.webos.service.ai.voice/stop '{}'
    {
        "returnValue": true
    }
    ```