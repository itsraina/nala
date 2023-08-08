# Nala
[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Are%20you%20a%20developer%20looking%20to%20learn%20how%20to%20build%20a%20voice%20assistant%20in%20Python?%20Check%20out%20Nala%20@%20https://github.com/jim-schwoebel/nala.&hashtags=voicecomputing,hackvoice,nala)

Nala is an agile open-source voice assistant framework to improve the workflow of your daily life. 

![](https://media.giphy.com/media/VDzVG8lvNRufu/giphy.gif)

Nala uses actions which can be triggered by user voice queries. All the user needs to do is say 'hey nala' and it will spark Nala to listen and respond to requests - like getting the weather or the news.

And yes, her name is inspired after Nala from the Lion King :-) 

See a newer version of [Nala here](https://github.com/jim-schwoebel/nala_assistant)

## Getting started

It's super easy to setup Nala. All you need to do is:

    git clone git@github.com:jim-schwoebel/nala.git
    cd nala
    python3 -m venv env
    source env/bin/activate
    python3 setup.py
    python3 nala.py
    
You will then be asked to register with your name, email, and a few other [registration tasks](https://github.com/jim-schwoebel/nala/wiki/3.-Registration).

After that, you're ready to begin using Nala! 

## How to query Nala

![](https://github.com/jim-schwoebel/nala/blob/master/data/other/Webp.net-gifmaker.gif)

### Single queries 

To active Nala, all you need to do is query her with 'Hey Nala!' (1) - which then triggers a response from Nala - (3) in this case, “How can I help you?.” Then, a user provides another query (usually after some beeping sound) - such as (4) “I’d like the weather.” Nala transcribes this query to understand it, and parses the query for keyword intents; for example, if the response is “I’d like the weather” the only word that really matters is “weather” and that would be used to provoke a response (5). Then, after this keyword maps onto an action dictionary (or a map of responses to keywords), the action is executed (6). Then, the intent loop repeats itself, looking for another wakeword (“Hey Nala”) before triggering another action. 

### Multi-query capability 

Nala is equipped with multi-query capability. All you need to do is add 'AND' into your query and she'll automatically execute actions serially that you request to her. 

For example, you may say, "Hey Nala" --> "close spotify and sleep" 

She will then close spotify and then go to sleep for 30 minutes. 

This makes Nala incredibly versatile to do multiple things quickly and is an advantage over other chatbot systems. 

## Demo (click video below)
[![multiple intents](https://github.com/jim-schwoebel/nala/blob/master/data/other/Screen%20Shot%202018-08-02%20at%202.36.25%20PM.png
)](https://drive.google.com/open?id=1Ubeyxot4G6oVXXt0REPfPLSwA29Hpliz "Querying multiple intents - Nala")

## What Nala can do 
Here are some actions that Nala can currently do along with the query intents needed to activate them. If you have any other ideas, let us know on the [github issues tab](https://github.com/jim-schwoebel/nala/issues) (as an enhancement)! 

| Action  | Description | Example query intent | 
| ------------- | ------------- | ------------- |
|⏰ alarm.py | Plays an alarm sound (e.g. to wake up in morning) based on the time of day you specified during user registration. | “set alarm”, “stop alarm” | 
|🎵 chillout.py | Plays music in the background to help you calm down.| “chill out” | 
|🏟️ espn.py | Scrapes ESPN website to find any events going on later tonight. This is a work-in-progress.| “get sports”|
|🎴 events.py | Scrape meetup.com for events in your local area. | “find events” | 
|📜 generate_poem.py | Generate a poem based on the generate poetry script we wrote a while back.| “make a poem”| 
|📝 grateful.py | Helps you keep a gratitude journal by recording a sample of what you’re grateful for today. | “be grateful” | 
|☺️ makeajoke.py | Plays back a joke from the database. | “make a joke” | 
|🌅 meditation.py | Guides you through a simple 60 second meditation.| “meditate” | 
|🎧 music.py | YouTube music links - based on a genre. | “play music” | 
|📰 news.py | searches some basic news sites related to computer science and machine learning (e.g. Hacker News). | “grab the news” | 
|🍐 nutrition.py | Searches for some healthy food nearby | “be healthy” | 
|✈️ plan_trip.py | Schedules a trip in terms of AirBnB suggestions and flights | “plan trip” | 
|↪️ reboot.py | Restarts the computer. | “restart” |
|🔍 search.py | search bing with a query. | First query: “search”, Second query: [search term] | 
|⌛ shutdown.py | Shuts down the computer. | “shut down” |
|😴 sleep |  Puts the computer to sleep for a designated time period. | "go to sleep"|
|👥 social.py | Alternative script to give you some suggestions based on your budget to go out later. | "be social"|
|🌡️ weather.py | Searches weather.com for the current weather at your location. | "get the weather"|
|☕🍦🎉🍺 yelp.py | Based on the query, searches yelp for coffee, restaurants, food, nightlife, ice cream, or bars. |"get me coffee", "get me some food", "nightlife", "get ice cream", "grab beer"| 
|📂open program | GitHub, Facebook, LinkedIn, Twitter, Spotify, Sublime, Atom |"open github", "open facebook", "open linkedin", "open twitter", "open spotify", "open sublime", "open atom"|
|📴close program | Close a Spotify session. | "close spotify", "stop spotify"|
|🎙️Record audio | record a stream of audio for a designated time period and save to desktop | "record audio" | 
|📹Record video | Open up zoom meeting link to record a video session. | "record video" | 

... more to come into the future! 

## Sample Projects

Here are some other projects that have used the Nala Framework:

* [Greta](https://github.com/protea-earth/greta) - 👧 Greta is an agile voice assistant to help reduce your carbon footprint.

## Feedback
Any feedback this repository is greatly appreciated. 
* If you find something that is missing or doesn't work, please consider opening a [GitHub issue](https://github.com/jim-schwoebel/nala/issues).
* If you want to learn more about voice computing, check out [Voice Computing in Python](https://github.com/jim-schwoebel/voicebook) book.
* If you are looking for a framework to start building machine learning models in voice computing, check out [Allie](https://github.com/jim-schwoebel/allie).
* If you'd like to be mentored by someone on our team, check out the [Innovation Fellows Program](http://neurolex.ai/research).
* If you want to talk to me directly, please send me an email @ js@neurolex.co. 

## License
This repository is licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). 

## References 

If you need anything else, check out [the wiki](https://github.com/jim-schwoebel/nala/wiki). 

If you're looking for a place to start to learn how to code voice computing, Nala has some great documentation in [Chapter 7 of the Voicebook repository](https://github.com/jim-schwoebel/voicebook/tree/master/chapter_7_design).

Here are some other modules and things you could look into for further guidance:

* [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
* [Google speech API](https://cloud.google.com/speech-to-text/docs/)
* [Pyttsx3](https://github.com/nateshmbhat/pyttsx3)
* [Pocketsphinx](https://github.com/cmusphinx/pocketsphinx)
* [Porcupine](https://github.com/Picovoice/Porcupine)
* [Sounddevice](https://python-sounddevice.readthedocs.io/en/0.3.11/)
* [Soundfile](https://github.com/bastibe/SoundFile)
* [SpeechRecognition](https://pypi.org/project/SpeechRecognition/) 
* [Voicebook](https://github.com/jim-schwoebel/voicebook/tree/master)
