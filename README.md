# Big G Express: Predicting Derates

Presentation: https://docs.google.com/presentation/d/1USJeeOm9EeSrvLZr2YvWj7XL0xTf3zeIDKNPqeW94VE/edit?usp=drive_link

<ins> **Background: **</ins>

This project delves into J1939 fault code data and vehicle onboard diagnostic data to try and predict an upcoming full derate. 

J1939 is a communications protocol used in heavy-duty vehicles (like trucks, buses, and construction equipment) to allow different electronic control units (ECUs), like the engine, transmission, and brake systems, to talk to each other. Fault codes in this system follow a standard format so that mechanics and diagnostic tools can understand what's wrong, no matter the make or model.

These fault codes have two parts. First, an SPN (Suspect Parameter Number), which identifies what system or component is having the issue. Second, an FMI (Failure Mode Identifier), which explains how the system is failing (too high, too low, short circuit, etc.).

A derate refers to the truck's computer intentionally reducing engine power or speed to protect itself or force the driver to get it serviced. This is a built-in safety measure. A full derate, the main target in this project, means the vehicle is severely limited, requiring a tow for repairs. Full derates are indicated by an SPN of 5246. 