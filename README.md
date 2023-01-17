# Introduction

Hurry is a situation when the QB is forced to throw the ball earlier than intended or is chased around/out of the pocket as the result of defensive pressure. To prevent this, the offensive line protects the passer, providing precious seconds to find receivers downfield. We decided to find out how the amount of time a quarterback has to throw the ball affects the outcome of a pass.

# Methodology

`Decision Time` is calculated as the number of seconds between the ball snap and the moment the first player on the defensive team gets within 3 yards or closer of the quarterback.

With the help of statistical tests, we investigate the influence of the following factors on the result of a pass.

* The fact that the defense players got close to the quarterback.
* Amount of time the QB has to throw the ball.

# Steps

1. Data loading, EDA: Selection of the parameters needed for the study. Exploring the possible outcomes of a play.
2. Creation of functions to calculate
* distance from defense players to QB;
* moment a defensive player gets close to the QB.
3. Calculation of the desired time parameters for all available games.
4. Examining differences
* in pass results between two samples (Close / not Close);
* in decision times between two samples (Complete pass / Incomplete pass).
5. Introducing new metric: Decision Time

# Results

We have found that there is a relationship between the time spent to make a decision and the result of the pass.

The faster the quarterback decides to throw the ball, the more likely it is that the pass will succeed. A bad block by offensive linemen means that the quarterback, in addition to finding the right receiver, has to spend time dodging defensive linemen. This increases the chances of an incomplete pass.

# Applicability of results

We introduce a new metric: `Decision Time`.

* It can be used to evaluate both the success of the offensive linemen in restraining the attack of their opponents, and the effectiveness of breaking through the block by the linemen of the defense.
* Coaches can use this data to plan strategies for upcoming games by considering the average `Decision Time` per team/season.

This metric will also be intuitive to the viewer. Its values are easy to compare and can be considered within the framework of both pre-game and post-game statistics. For example:

<table border="1" align="center">
  <tr>
    <th>Before the game between MIA and TB</th>
    <th>After the game between DAL and TB</th>
  </tr>
  <tr>
    <td height=500 width=500><img src="https://github.com/ryan4waters/NFL-Big-Data-Bowl-by-Practicum/blob/DECISION_TIME_MATTERS/figures/Before%20the%20game%20between%20MIA%20and%20TB.png" alt="" height=500 width=500 /></td>
    <td height=500 width=500><img src="https://github.com/ryan4waters/NFL-Big-Data-Bowl-by-Practicum/blob/DECISION_TIME_MATTERS/figures/After%20the%20game%20between%20DAL%20and%20TB.png" alt="" height=500 width=500 /></td>
  </tr>
</table>