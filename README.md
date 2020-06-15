# signal_processing_distance_between_devices

Different methods have been used to find the distance between two smart devices using information generated from GPS, Gyroscope,
Bluetooth, and compass. In this project, we are working on the signal processing part of a model which uses sound and works for any
device which has a microphone and a speaker.
In this model, round trip sound time of two note sequence is calculated. First, the two devices communicate and then the pinger plays
the first note - PING. The second device receives the ping and waits for a delay of ‘d’ and then replies with the second note - PONG. Once
the pinger detects the pong at a certain time, the distance between the two devices can be calculated using the speed of sound.

Here, the first task is to detect the ping signal. But using a tuned frequency detector would be too slow for the purpose. So we need to
use an onset detector which will then trigger the tuned frequency detector. In this project, we have made matlab models for the two
detectors and analysed their working.
