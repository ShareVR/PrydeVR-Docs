# Introduction
With a goal of providing the most intuitive interaction experience, we have implemented multiple ways of engaging with Pryde's functionality.

---

## Speech Interface
You are in the middle of a game session, shooting your enermies while trying to cover your teammates, such a wonderful moment for you to capture with Pryde so you can easily show it off to your friends, you looked at your hand and realized that all of your keys has been mapped already, leaving you no easy way to tell the Pryde camera to start recording. Wait, how about just TALK TO THE CAMERA? That will easily solve the problem, right?

The litle scenario above is one of the main reason why we introduced the speech interface. With the Pryde speech interface, you can simply talk to Pryde to control functions like start/stop recording, show/hide camera preview panel, *etc.*


!!! note
    Do you feel like an idiot when trying to talk to the computer/device multiple times and then absolutely nothing happens? Well we feel the same. That's why we have put extra amount of work to ensure that this just works like a charm. In order to provide butter smooth experience of voice interaction with both low latency and great accuracy, we are using native Windows speech API which is part of the Windows 10 OS. Aside from latency and accuracy, this also have the benefit of not requiring Internet connection at all so don't worry about privacy or bandwitdh. However, using such API does have one requirement, you do need to be using Windows 10 OS. So if you are testing this using MacOS or Linux, please turn speech interface off.

### Available Commands List
Below is a list of all of available voice commands. Note that we have multiple alternatives for each command action so you can pick one that works for you the best, *i.e.* has the lowest error rate. **-** means the same command as above.

| Command Action | Voice Command (Say it out loud) |
| :------------: | :-----------------------------: |
| Start Recording | *start*  |
| - | *start recording* |
| - | *begin recording* |
| - | *redording start* |
| Stop Recording | *stop* |
| - | *stop recording* |
| - | *ternimate recording* |
| - | *finish recording* |
| - | *end recording* |
| - | *recording stop* |
| Show Camera Model | *show camera* |
| - | *enable camera* |
| Hide Camera Model | *hide camera* |
| - | *disable camera* |
| Switch Camera to Smooth Follow Mode | *camera follow* |
| - | *follow me* |
| Switch Camera to Orbit Mode | *camera orbit* |
| - | *orbit me* |
| Show Avatar | *show avatar* |
| - | *enable avatar* |
| - | *avatar on* |
| Hide Avatar | *hide avatar* |
| - | *disable avatar* |
| - | *avatar off* |

---

## Keyboard and Controller Trigger
If you do have an extra key on the controller or keyboard, we have reserved the key trigger functionality so you can assign one or a combination of two keys to trigger recording start/stop.

---

## API Interface
Future managed external Unity API interface has been planned and we will have a beta version shipped to be tested soon. Stay tuned!
