# AWPX4HX-2023
This collection of all weather, PX4, Hexacopter, 2023 Annotated flight logs is a work in progress. The dataset will be continually updated and released as a standard benchmark dataset by December 15th, 2023. However, we make it available for use in the meanwhile. 

@Nafee, you need to create something like this:
https://github.com/SAREC-Lab/sUAS-UseCases/edit/FSE2021-HumanInteractionHazards/README.md

For convenience, I've copied that markdown file below:

# Flight log attributes

Describe the attributes here. 

# Environmental attributes

Describe them here. Create a table and add icons from your ppt presentation.

# Annotated Anomalies with Explanation

Provide an example

# Flight logs
All flight logs are currently available on google drive, but will be reorganized and ported to github shortly.
[flight logs](https://drive.google.com/drive/folders/1DoAreav--ewsFONFb40o4TuOCK8ZddvQ)

@Nafee, let's discuss this. I would suggest a table format which summarizes each flight log very cleanly and provides a link to the logs.px4 and a downloadable zip file.  (You can add more later, but I think that is best for this intermediate release).  The table should be really informative.


@Nafee, the following is just an example from another page we created

The following hazards have been derived from a systematic study of publications reporting safety analyses techniques applied to the domain of small Unmanned Aerial Vehicles. They are supported by a [glossary of terms](glossary.md).  We are currently [eliciting feedback](feedback.md) on this hazard trees.

For a detailed description of the process and the different Hazard Catetories please see our paper [Hazard Analysis for Human-on-the-LoopInteractions in sUAS Systems](FSE_2021_HumanInteractionPoints_AcceptedVersion.pdf) at the 29th ACM Joint European Software Engineering Conference and Symposium on the
Foundations of Software Engineering


If you would like to use these Hazard Trees we ask you to reference our paper:

Michael Vierhauser, Md Nafee Al Islam, Ankit Agrawal, Jane Cleland-Huang,and James Mason. *Hazard Analysis for Human-on-the-Loop Inter-actions in sUAS Systems.* In Proceedings of the 29th ACM Joint EuropeanSoftware Engineering Conference and Symposium on the Foundations of Soft-ware Engineering (ESEC/FSE ’21). ACM,New York, NY, USA, 12 pages. https://doi.org/10.1145/3468264.3468534


### Hazard Types

We have organized them into trees of related hazards. Our focus here is on exploring human-drone interaction hazards. Usage suggestions can be found [here](usage.md).

For each identified human-drone interaction point, we explore four specific types of hazards: 
<br> <sub>[![](human-interaction-hazards/icons/h-icon.PNG)](#) </sub> -  Human Initiated Hazards (e.g., the RPIC flies whilst inebriated, ignores regulations, and/or behaves in a reckless manner)
<br> <sub> [![](human-interaction-hazards/icons/s-icon.PNG)](#) </sub> - Loss of Situational Awareness, including lack of information and/or comprehension about the state of current/intended mission 
<br> <sub> [![](human-interaction-hazards/icons/e-icon.PNG)](#) </sub> - Lack of Empowerment to intervene in the situation (e.g., inability to override an autonomous decision made by a UAV)

### Hazard Groupings

| Hazard Group | Description |Link to Hazard Information ||
|:--|:--| :--|:--|
|HG1 - Collisions| Hazards related to collisions between multiple UAVs and/or UAVs and other objects|[collisions.md](human-interaction-hazards/collisions.md)|:heavy_check_mark:|
|HG2 - Communication| Loss of communication with the UAV |[communication.md](human-interaction-hazards/communication.md)|:heavy_check_mark:||
|HG3 - Hardware/Sensors| Hardware and sensors |[sensors.md](human-interaction-hazards/sensors.md)|:heavy_check_mark:|
|HG4 - Mission Awareness|Hazards associated with general situational awareness and operator empowerment during a mission| [missionawareness.md](human-interaction-hazards/missionawareness.md)|:heavy_check_mark:|
|HG5 - Mission Planning| Hazards related to planning and managing flight routes |[missionplanning.md](human-interaction-hazards/missionplanning.md)|:heavy_check_mark:|
|HG6 - Preflight Configuration|Prelaunch hazards|[preflightchecks.md](human-interaction-hazards/preflightchecks.md)|:heavy_check_mark:|
|HG7 - Regulatory Compliance| Hazards related to flight authorization and other regulations|[prohibited-airspace.md](human-interaction-hazards/prohibited-airspace.md)|:heavy_check_mark:|
|HG8 - Weather related| Weather related hazards |[weather.md](human-interaction-hazards/weather.md)|:heavy_check_mark:||


### Dataset

We provide a hierarchical structured Hazard Tree for each of the groups as described above.
In addition to the graphical representation, we provide a textual representation of all trees as a dataset. Text files can be found in the folder [trees](/trees).
The dataset contains the same information as shown in the hazard trees on GitHub and information is encoded as follows:

System hazards are marked with the prefix ``h`` (e.g., h1) and user-interaction hazards are named according to their group (e.g. ``wx1`` for a user-interaction hazard in the hazard group weather), and are taged with the hazard type (e.g., ``[h]`` for human initiaed error).
The hierarchy is established via the map tag (e.g., ``map h1 h2`` means that ``h2`` is a child hazard of ``h1``)


[Return to Dataset overview](https://github.com/SAREC-Lab/sUAS-UseCases/blob/master/README.md)
