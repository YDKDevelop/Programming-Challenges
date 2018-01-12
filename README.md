# Programming-Challenges
My solutions for dailyprogrammer challenges

## Requirements

- Python 3
  - praw
  - pprint

## Installation

  ```bash
  $ pip3 install -r etc/requirements.txt
  ```

## How to use

The script can also be run via the command line by running `./post-challenges.py <number_of_challenges>`
It will look for a copy of `praw.ini`, an example is in `etc/praw.ini.example`

You may wish to run this in a temporary directory, to avoid adding folders directly to the top directory of the repo. Move the various levels of challenges into their respective end points.

### Example full run

  ```bash
  $ cd DailyProgrammerChallenges
  $ mkdir tmp
  $ cp etc/praw.ini.example tmp/praw.ini
  $ cd tmp
  # Edit praw.ini with the correct info
  $ ../post-challenges.py
  # Take a look at what was downloaded for any 'problems'
  $ mv *Easy* "Easy Challenges/."
  $ mv *Intermediate* "Intermediate Challenges/."
  $ mv *Hard* "Hard Challenges/."
  $ cd ..
  $ ./transform.py
  ```

  Examine the changes that `transform.py` performed and check that they seem okay.



