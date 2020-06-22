# Capstone: Check In 1

### Contents:
- [Idea 1: Music Composition](#Idea-1)
- [Idea 2: Predict the Age of Shellfish](#Idea-2)
- [Idea 3: Pittsburgh Bridges](#Idea-3)

<a id=Idea-1></a>
## Idea 1: Music Composition

#### Data Source: 
UCI http://archive.ics.uci.edu/ml/datasets/Bach+Chorales

#### Goal: 
Learn a generative grammar for stylistically valid chorales. Predict pattern for the style of a musical composition. 

#### Problem Statement:
The grand challenge is to learn a generative grammar for stylistically valid chorales (see references and discussion in "Multiple Viewpoint Systems for Music Prediction").

#### Audience:
Classical music enthusiasts who want to know the recipe

#### Success Metric:
Provide the features and components that make up a classical music composition

#### Attributes:
(a) start-time, measured in 16th notes from chorale beginning (time 0) <br>
(b) pitch, MIDI number (60 = C4, 61 = C#4, 72 = C5, etc.)<br>
(c) duration, measured in 16th notes<br>
(d) key signature, number of sharps or flats, positive if key signature has sharps, negative if key signature has flats<br>
(e) time signature, in 16th notes per bar<br>
(f) fermata, true or false depending on whether event is under a fermata<br>

<a id=Idea-2></a> 
## Idea 2: Predict the Age of Shellfish

#### Data Source:
http://archive.ics.uci.edu/ml/datasets/Abalone

#### Goal:

Predict the age of a seashell

#### Attribute Information:
Given is the attribute name, attribute type, the measurement unit and a brief description. The number of rings is the value to predict: either as a continuous value or as a classification problem.

Name / Data Type / Measurement Unit / Description
-----------------------------
Sex / nominal / -- / M, F, and I (infant)<br>
Length / continuous / mm / Longest shell measurement<br>
Diameter / continuous / mm / perpendicular to length<br>
Height / continuous / mm / with meat in shell<br>
Whole weight / continuous / grams / whole abalone<br>
Shucked weight / continuous / grams / weight of meat<br>
Viscera weight / continuous / grams / gut weight (after bleeding)<br>
Shell weight / continuous / grams / after being dried<br>
Rings / integer / -- / +1.5 gives the age in years<br>

#### Problem Statement:
How old is this seashell?

#### Audience:

Marine biologists and beach shell collector enthusiasts

#### Success Metric:

Determine the age of a seashell

<a id=Idea-3></a>
## Idea 3: Pittsburgh Bridges

#### Data Source: 
UCI https://archive.ics.uci.edu/ml/datasets/Pittsburgh+Bridges

#### Goal:  
5 properties (design description) need to be predicted based on 7 specification properties

#### Problem Statement:
What are the properties of iconic bridges?

#### Audience:
Bridge enthusiasts. Civil engineers.

#### Success Metric:
Find the properties of iconic Pittsburgh bridges

#### Attributes:
(Attribute Information:
The type field state whether a property is continuous/integer (c) or nominal (n).

For properties with c,n type, the range of continuous numbers is given first and the possible values of the nominal follow the semi-colon.

Name / Type / Possible values / Comments

1. IDENTIF / -- / -- / identifier of the examples
2. RIVER / n / A, M, O / --
3. LOCATION / n / 1 to 52 / --
4. ERECTED / c,n / 1818-1986 ; CRAFTS, EMERGING, MATURE, MODERN / --
5. PURPOSE / n / WALK, AQUEDUCT, RR, HIGHWAY / --
6. LENGTH / c,n / 804-4558 ; SHORT, MEDIUM, LONG / --
7. LANES / c,n / 1, 2, 4, 6 ; 1, 2, 4, 6 / --
8. CLEAR-G / n / N, G / --
9. T-OR-D / n / THROUGH, DECK / --
10. MATERIAL / n / WOOD, IRON, STEEL / --
11. SPAN / n / SHORT, MEDUIM, LONG / --
12. REL-L / n / S, S-F, F / --
13. TYPE / n / WOOD, SUSPEN, SIMPLE-T, ARCH, CANTILEV, CONT-T / --


