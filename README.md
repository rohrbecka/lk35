# LK35
LK35 is an application to control multicolor LED room lighting.

## Requirements Overview
LK35 is an application to control multicolor LED room lighting, which is controlled through an [LK35 LED-Controller](http://www.led-studien.de/2014/07/28/wlan-rgbw-controller-lk35-mit-api/). The main features of the application are
* Support of LK35 Controller with RGB, RGBW, WW/CW or White-Only LED-Strips
* Definition of different Sites with an arbitrary number of controllers
* Grouping of controllers
* Available for macOS, iOS, watchOS and tvOS
* Different controllers for setting the colors including
  - Color Wheel
  - Dimmed White
  - Dimmed White with Color Temperature Control
  - Favorites
* Synchronisation through iCloud
* Export / Import of Site Settings

LK35 is intended to be published in the iOS and the macOS App Store. It should support:
* macOS 10.12 Sierra
* iOS 10
* watchOS 3
* tvOS 10

As LK35 is a side-project of André Rohrbeck it is developped not only for controlling the lights at home, but also as educational project to learn Swift, which is used as Swift 3.

## Quality Goals

* Rapidity of Use
  LK35 is used to set the room lighting. Nobody wants this to be complicated or last long (LK35 is competing with a light switch on the wall). The interaction for switching the light in the desired room into the desired lighting should therefore be no longer than 2 seconds.
* Ease of Use
  After being set up, the operation of the lights should be very easy and non-technical (nobody expects to know a URL to switch on the light).
* Adaptation to the Platform
  The different platforms (macOS, iOS, watchOS, tvOS) have different usage scenarios (e.g. nobody will switch on his TV in order to switch off the room light). These scenarios should be used to define which features of the applications will be provided for which platform. E.g. as an Apple Watch is always coupled to an iPhone it makes no sense to set up the controllers on the Watch as nobody wants to enter IP adresses through the digital crown. Instead the Watch is relying on iCloud sync and that the setup was done through an iPhone or a Mac.
* Swiftness
  Finally LK35 is also intended as an educational project to explore Swift best practices. It should therefore strictly follow Apple Guidelines (especially the Swift API guidelines) and use a "Swift" approach of solving the programming problems.
* Tests
  A side-goal of the project is to explore the testability of applications. A test coverage of at least 90% shall therefore be achieved. Additionally also the UI should be tested.
* Expandability
  As the project is only at its beginning it should be designed with extensions in mind. These may be feature extensions like a different light controller than the LK35, an additional user interface (e. g. to define light sequences or to generate lighting based on sounds recorded by the microphone) or better accessibilty by providing Speech Control through Siri. "Hey Siri, switch on romantic lighting in the living room!"


## Stakeholders
In the first place LK35 is a personal project of André Rohrbeck to control the lights at home and to improve the programming skills for the Apple platforms and with Swift 3. Therefore André is the main Stakeholder of the project. Nevertheless others are existing or may exist:

* LED-Studien, Nino Turianskyj
  Nino and his company are the provider of the LK35 controller and should therefore have an interest in providing information about the LK35 application. Finally his product should profit of the availability of a great application on the Apple platforms. On the other hand he could also contribute to the project by making the setup process easier (e.g. by providing controllers with Bonjour capabilities).

* Contributors
  I am not expecting many people to contribute to the project, but of course everybody is invited to improve the codebase or to join me developping new features for the application as long as he/she is supporting the quality goals outlined above.

* Users
  The users of the application should be the main source of feedback. As users are usually only complaining and not often stating, which features are great, the users should be motivated to give their feedback to make LK35 the best lighting app available.
