# RegoAI

* This project is the development of an AI that can play the Blokus board game through algorithms and machine learning.
* Through appropriate sorting algorithms and pruning of weaker moves, RegoAI aims to have multiple variables that determine aggression, maximization of perceived area and the blocking of enemy piece vertices.
* Similar to Stockfish, an evaluation bar will be able to determine the approximate game state for each player.

  * [License](#license)
  * [Frequently Asked Questions](#frequently-asked-questions)
  * [Planned Features](#planned-features)
  * [Release History](#release-history)
  * [Contributions](#contributions)
  * [Bugs](#bugs)

## License

### GNU GPLv3

> I *do not own or profit off* of Blokus©, the intellectual property of Mattel© and this project does not reflect the ideas or beliefs of Mattel© or any other intellectual property owned by Mattel©. All other product names and associated designs are trademarks and copyrighted properties of their respective owners. ©2013 Mattel. All Rights Reserved.
>

## Frequently Asked Questions

* WIP

## Planned Features

* Bound by 20 x 20 tile grid (400 tiles <sup>2</sup> )
* Only allow player starts be from the corner
* Only allow piece vertex collision
* Have each piece be its own variable
* Place all pieces on the board to minimise score

  `(best score is 0; each player starts with 89 points [w])`

* Decide on which algorithm to use (depth/best first)
  * Monte Carlo Search Tree
  * minimax (4 player ?)
  * Heuristic Search (Machine Learning)
  * Multiplayer alpha beta pruning
  * Combinatorial Game Theory
  * A* Depth First Search

* Develop an AutoSolver in the endgame (10 > moves available)
  * Skip function if no moves are available

* **Evaluation algorithm** :

> Increase "m" score if approaching middle
>> +1 if in (20 x 20) - (10 x 10) of square
>>
>> +2 if in the (10 x 10) - (4 x 4) outline inside
>>
>> +3 if in the 4 x 4 middle
>
> Decrease "p" score when using -5 pieces
> 
> Increase "e" score if % area of 20x20 where x > 25%
>> Area will always be within 400 t <sup>2</sup>
>>
>> Use of integration for wave-like functions or pythagoras for right-angled triangles or length x width
>>
>> How can I maximize inward facing vertexes?

* Find a way to condense games into simplifed form similar to Chess
* Aggression metre through AI behaviour to limit opponent block verticies
* Pattern recognition through learning to block incoming threats and pressure
* UI/UX

## Release History

* 0.0.3 (2022-10-01)
  * Created red, green, blue, yellow polyomino assets for RegoAI
* 0.0.2 (2022-09-29)
  * Discussed development plan and gathered advice from university professors on how to execute the project.
* 0.0.1 (2022-09-20)
  * Officially began development

## Contributions

Refer to the Contributing.md file located in the root file of RegoAI.

## Bugs

Currently no known bugs. (wow)
