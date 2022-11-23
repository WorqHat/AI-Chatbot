# A Simple Voice AI Bot with Web Speech API and Node.js

This demo uses the experimental Web Speech API, which is currently only [supported](http://caniuse.com/#search=speech) by Blink-based browsers including Chrome 25+, Opera 27+, Samsung Internet, QQ Browser, and Baidu Browser.

![Demo Image](https://i.vimeocdn.com/video/633160262_480x297.jpg)


This is how this web application works:

1. Using the Web Speech API’s `SpeechRecognition` interface to listen your voice from a microphone
2. Send your message to [API.ai](https://api.ai) (the natural language processing platform) as a text string
3. Once the AI from the API.ai returns the reply text back, use the `SpeechSynthesis` interface to give it a synthetic voice.




### Try It on Your Own Server

Rename the `.env.local` to `.env` and fill the env vars:

```
APIAI_TOKEN=
APIAI_SESSION_ID=some_unique_session_id
```

The first one is an API.ai API key (Please get one by sign up with [API.ai](https://api.ai)), and the second one is a session ID, which is an arbitrary string (we could make this unique within the app, but that's beyond the scope of this demo).
