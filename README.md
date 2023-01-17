# Introduction

Hurry is a situation when the QB is forced to throw the ball earlier than intended or is chased around/out of the pocket as the result of defensive pressure. To prevent this, the offensive line protects the passer, providing precious seconds to find receivers downfield. We decided to find out how the amount of time a quarterback has to throw the ball affects the outcome of a pass.

# Methodology

Decision Time is calculated as the number of seconds between the ball snap and the moment the first player on the defensive team gets within 3 yards or closer of the quarterback.

With the help of statistical tests, we investigate the influence of the following factors on the result of a pass.

- The fact that the defense players got close to the quarterback.
- Amount of time the QB has to throw the ball.

# Steps

1. Data loading, EDA: Selection of the parameters needed for the study. Exploring the possible outcomes of a play.
2. Creation of functions to calculate
- distance from defense players to QB;
- moment a defensive player gets close to the QB.
3. Calculation of the desired time parameters for all available games.
4. Examining differences
- in pass results between two samples (Close / not Close);
- in decision times between two samples (Complete pass / Incomplete pass).
5. Introducing new metric: Decision Time

# Applicability of results

We introduce a new metric: Decision Time.

- It can be used to evaluate both the success of the offensive linemen in restraining the attack of their opponents, and the effectiveness of breaking through the block by the linemen of the defense.
- Coaches can use this data to plan strategies for upcoming games by considering the average Decision Time per team/season.

![image]()

|Before the game between MIA and TB|After the game between DAL and TB
|
|:---:|:---:|
|2|1|