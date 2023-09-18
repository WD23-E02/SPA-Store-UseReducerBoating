# A boat with useReducer
[![Status overview badge](../../blob/badges/.github/badges/main/badge.svg)](#-results)


I want you to create a boat interface using `useReducer`.
You don't need to make many different components, but your UI should have the following elements:

- "Start engine" button
    - When the button is clicked, the engine status text should display "engine on".
- "Gear up" button
    - When the button is clicked, and the engine is started, the current gear text should increment by 1 (max 5).
- "Gear down" button
    - When the "Gear down" button is clicked, and the engine is started, the current gear text should decrement by 1 (min -2).
-  "Accelerate" button
    - When the "Accelerate" button is clicked, and the engine is started and in a non-zero gear, the speed text should increment according to the current gear.


Your reducer function should be able to do the following actions:

- start the boat engine
- stop the boat engine
    - also resets gear to 0
    - does not change the boat speed
- change engine gear up
    - only works if boat is started
    - max gear 5
- change engine gear down
    - only works if boat is started
    - min gear -2
- increase boat speed
    - only works if boat is started
    - if gear is 0, has no effect
    - changes boat speed so that is further away from 0
    - gear 5 increases speed faster than gear 1
    - gear -2 increases speed faster than gear -1
- decrease boat speed
    - only works if boat is started
    - if gear is 0, has no effect
    - changes boat speed so that is closer to 0

Show the current speed of the boat to the user
Show also buttons for the different actions

**BONUS CHALLENGE** Show distance travelled

[//]: # (autograding info start)
# <img src="https://github.com/DCI-EdTech/autograding-setup/raw/main/assets/bot-large.svg" alt="" data-canonical-src="https://github.com/DCI-EdTech/autograding-setup/raw/main/assets/bot-large.svg" height="31" /> Results
> ⌛ Give it a minute. As long as you see the orange dot ![processing](https://raw.githubusercontent.com/DCI-EdTech/autograding-setup/main/assets/processing.svg) on top, CodeBuddy is still processing. Refresh this page to see it's current status.
>
> This is what CodeBuddy found when running your code. It is to show you what you have achieved and to give you hints on how to complete the exercise.


### Start Engine

|                 Status                  | Check                                                                                    |
| :-------------------------------------: | :--------------------------------------------------------------------------------------- |
| ![Status](../../blob/badges/.github/badges/main/status0.svg) | 'Start engine' button exists |
| ![Status](../../blob/badges/.github/badges/main/status1.svg) | Starts engine when clicked |

### Gear Up

|                 Status                  | Check                                                                                    |
| :-------------------------------------: | :--------------------------------------------------------------------------------------- |
| ![Status](../../blob/badges/.github/badges/main/status2.svg) | 'Gear up' button exists |
| ![Status](../../blob/badges/.github/badges/main/status3.svg) | Increments the gear by 1 when clicked |

### Gear Down

|                 Status                  | Check                                                                                    |
| :-------------------------------------: | :--------------------------------------------------------------------------------------- |
| ![Status](../../blob/badges/.github/badges/main/status4.svg) |  'Gear Down' button exists |
| ![Status](../../blob/badges/.github/badges/main/status5.svg) | Decrements the gear by 1 when clicked |

### Accelerate

|                 Status                  | Check                                                                                    |
| :-------------------------------------: | :--------------------------------------------------------------------------------------- |
| ![Status](../../blob/badges/.github/badges/main/status6.svg) | 'Accelerate' button exists |
| ![Status](../../blob/badges/.github/badges/main/status7.svg) | 'Increments the speed by 10 when clicked |



[🔬 Results Details](../../actions)
[🐞 Tips on Debugging](https://github.com/DCI-EdTech/autograding-setup/wiki/How-to-work-with-CodeBuddy)
[📢 Report Problem](https://docs.google.com/forms/d/e/1FAIpQLSfS8wPh6bCMTLF2wmjiE5_UhPiOEnubEwwPLN_M8zTCjx5qbg/viewform?usp=pp_url&entry.652569746=SPA-Store-UseReducerBoating)


[//]: # (autograding info end)