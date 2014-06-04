![System Diagram](../project_images/System Diagram.jpg?raw=true "System Diagram")

The idea is to get access to a live data stream from a radio telescope trained at a pulsar. The data needs to be transformed *somehow* so that I can use it to fire off the servos on the bio-pixels at an appropriate rate and in some interesting way. 

I will need to do some tests on the bioluminescent algae to find out what a reasonable interval between flashes is (apparently they get exhausted if they flash too often).

The data will be manipulated on the server and then sent via server sent events to the client devices. 

Each device will control a charlieplexed array of ‘bio-pixels’ - I’ll use LEDs for testing

A bio-pixel will be a small (~50mm) glass container containing seawater and an amount of dinoflagellates. A magnetic stirrer in the container will be activated by a servo with attached magnets outside the vial. When the stirrer is activated the water is agitated causing the algae to glow.

![Bio Pixel](../project_images/biopixel.jpg?raw=true "Bio Pixel")

**The result is that ~~light~~ electromagnetic waves emitted from a star millions of years ago cause microscopic organisms to emit ~~light~~ their own EM waves out into the universe.**

##Task list
- ~~Create a new MEAN stack project using angular-fullstack-generator~~
- Find a source of live streaming data from a radio telescope directed at a pulsar (consider fallback plans)
- Write server code to ingest live stream (test with mocks)
- Write server code to manipulate stream data
- Write server code to send manipulated data
- Write client side code to ingest server data
- Write client side code to control Arduinos
- Write Arduino code to control servos
- Create model bio-pixel array with LEDs
- Create actual size model bio-pixel
- Test properties of bioluminescent algae
