# Introduction
PIDMA enables users to collaboratively construct automation rules based on their normal phone usage. These rules are formalized in an IF-THEN format: IF an event triggers, AND conditions are true, THEN actions are performed. 


PIDMA is implemented with an Android app, and the [APK](https://drive.google.com/file/d/1g6ltSQwPKBAeo9fjUd8MHr9VqY6c_1su/view?usp=drive_link) is publicly available. The backend code will be released soon after the paper is accepted.

## Motivation
PIDMA's goal is to extract rules embedded in users' everyday interactions with their phones. The graphical user interface (GUI) operations represent the desired actions, while environmental triggers and conditions are inherent in the smartphone's context. 

PIDMA harnesses the powerful perception capabilities of smartphones, and the reasoning power of large language models (LLMs), to lower the barrier for end-users when constructing automation rules. 

## Key Features
PIDMA contains two main stages:

1. **In-situ demonstration**: The user demonstrates the actions they want to automate.
2. **Collaborative rule programming**: The user collaborates with the system to refine and formalize the rules.

PIDMA supports both passive and active contexts to trigger automation rules:

1. **Passive contexts** include time, location, and notifications. These are automatically collected when the system is triggered by the user.
2. **Active contexts** include camera input, screen activity, voice/text input, and gestures. These can be provided during either the demonstration or the programming phase, depending on the user's intent.

## Demo videos of PIDMA

The following two videos demonstrate two examples of the same rule (the difference is whether active context is input during the demo phase): If the camera contains dumbbells and the location is within the student dormitory, then open the dumbbell tutorial in the JEFIT app.

## Baseline system
Since existing mobile automation tools (such as iOS Shortcuts) lack templates for active contexts, we have implemented a [Baseline](https://github.com/Anony-PIDMA/baseline/) system, which allows users to construct rules through screen clicks and text input, refers to existing tools.

