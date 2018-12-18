# EspLock Plugin

Example config.json:

    {
      "accessories": [
        {
            "accessory": "EspLock",
            "name": "Front Door",
            "url": "your-custom-or-homegrown-service-url",
        }
      ]
    }

This plugin supports locks controlled by any custom HTTP endpoint via GET (to get state, either "locked" or "unlocked"), and POST (to set new state, same two values). The "lock-id", "username" and "password" parameters are passed along to "url" in each GET request. The same parameters plus "state" are passed along to "url" in each POST request.

See [Siri HomeKit Controlled ESP8266 Lock](https://blog.aprbrother.com/p/710)
