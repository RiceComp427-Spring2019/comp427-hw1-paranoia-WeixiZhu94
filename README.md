# <img src="http://www.rice.edu/_images/rice-logo.jpg" width=180> Comp427, Spring 2018, Homework 1
## Rational Paranoia
The homework specifications, as well as the corresponding course slide decks,
can be found on the [Comp427 Piazza](https://piazza.com/class/jqifhp864b37ju).
This assignment is due **Thursday, January 17 at 6 p.m.**

You will do this homework by editing the _README.md_ file. It's in
[MarkDown format](https://guides.github.com/features/mastering-markdown/)
and will be rendered to beautiful HTML when you visit your GitHub repo.

## Student Information
Please also edit _README.md_ and replace your instructor's name and NetID with your own:

_Student name_: Weixi Zhu

_Student NetID_: wz28

Your NetID is typically your initials and a numeric digit. That's
what we need here.

_If you contacted us in advance and we approved a late submission,
please cut-and-paste the text from that email here._

## Problem 1
- Scenario: {Stadium}
- Assumptions:
  - Other teams are willing to try dirty stuff to beat my team.
- Assets:
  - The fairness of each football game, which is guaranteed by the fact that
    all players are not affected by drugs. Since football game is sort of
    examining if the players are strong, taking drugs for the game is like
    cheating that will make the players banned.
  - The sports spirit of each football game, that players from all teams are
    trying to win instead of deliberately trying to lose. If players from a
    team try to deliberately lose scores and let the other team win, this is
    violating the sports spirit and making the game meaningless.
- Threats:
  - Malicious teams may try to use drugs to break the fairness and win the
    games. Drugs make athletes more excited and exhibit better strength in the
    games such that they can win the games easier.
  - Malicious teams may also exploit the fact that players using drugs will be
    banned from games. Therefore, they could secretly put drugs in opposite
    teams' food or drinks, letting them get tested to violating the fairness
    and banned from games.
  - Players may involve in gambling by betting their own teams' loss.
    Meanwhile, they participate in the games, trying to lose scores seemingly
    from mistakes but actually on purpose.
  - Referees may get biased and cater to one team in the game, which makes the
    game unfair.
- Countermeasures:
  - The stadium offers uranium test against drugs to avoid threat #1. This
    should be cheap and only requires hiring doctors with expertise.
  - The stadium can offer both food and drinks free from drugs. Additionally,
    people can still put drugs into open food or water bottles. In response,
    the stadium can put monitors to cover all places. Therefore, teams can
    freely enjoy food and drinks without getting drugs put in by malicious
    opposite teams. Putting monitors is cheap, but detecting if malicious
    people are putting drugs in other people's food is hard and costly. The
    benefit is that it can psychologically prevent people doing that malicious
    thing.
  - The stadium can selectively hire referees who have no conflict of
    interests with both teams. This only involves some investigation that
    would be cheap.
  - The stadium may ask experts tell from the game if players are trying to
    lose the game on purpose. If so, investigations can start on whether they
    involve in gambling. The second step is costly but the first step may
    effectively prevent people doing that.

## Problem 2
- Scenario: {Grading}
- Assumptions:
  - Some students are willing to take the risk of violating honor code.
- Assets:
  - The data integrity of submitted homework. Submitted homework must not be
    further modified. If the author wants to modify it, it is passing the
    submission deadline. If other people maliciously modify it, the data
    integrity is broken.
  - The confidentiality of submitted homework. If early submitted homework was
    seen by other people, they can borrow the idea of it and apply to their
    homework.
- Threats:
  - People can watch whatever homework was submitted on the network. Based on
    early submitted homework, they can steal the ideas or solutions from
    others.
  - People can intercept the homework being submitted on the network and
    submit another modified version instead. Therefore, they can make other
    people's submission worse and make their scores relatively higher.
- Countermeasures:
  - The data integrity can be protected by calculating a hash value of the
    submitted file. The student must submit their homework along with the
    computed hash code, by SHA256 algorithm for example. This is easy and
    there are existing tools to compute it. The grader then computes the hash
    value again and compare with the submitted work, if they do not equal then
    ask the students to submit again. Otherwise, send a confirmation email to
    the students.
  - The data confidentiality can be protected by encrypted submission channel
    on the network. Students must submit their homework by ssh where the
    communications via the network is encrypted. This is also cheap and they
    just need to learn via Google.

## Problem 3
- Scenario: I am overseeing the server for an online video game.
- Assumptions:
  - People always want to cheat the game without paying money or time.
- Assets:
  - The value of the virtual concurrency of the game.
  - The fairness of the game, when there are players vs. players or teams
    fighting for the first kill of some game bosses.
- Threats:
  - People can hack the game and when they attack the monsters, the hacked
    game client would falsely send messages that their damage is high enough
    to kill the monsters. So that the data integrity is broken.
  - People can further exploit some vulnerability of the game and replicate
    the game concurrencies to make money. However, this will quickly
    depreciate other players' belongings and ruin the game.
- Countermeasures:
  - Keep updating the game and fixing the vulnerabilities. At the same time,
    monitor the game market and the fluctuations of the values of game
    concurrencies. Always be ready to recover the game to some checkpoint if
    some disasters are happening. The updating and monitoring things could be
    cheap. The developers are hired for updating the game and making tools to
    help monitor. Recover the game back to older checkpoints could hurt the
    market and cost a lot, because players would be mad and quit the game.

