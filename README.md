# Weekly challenges for Xteam members

## Motivation
This programm is founded with the aim to train Xteam members' coding skills. Everyone in the team can contribute, by:
- Pull request your own solution (if you're really proud of it)
- Pull request new challenges. Your challenge could be from any coding languages, ranged from all levels.

## Challenges included
<ul>
    {% for challenge in site.challenges %}
        <li>
            <a href="{{ challenge.url | prepend: site.baseurl }}">{{ challenge.title }}</a>
        </li>
    {% endfor %}
</ul>

<!-- ### ReactJS
- Level: Easy
    - [Color code's guessing game]({{site.baseurl}}/react-guessColorCode)
- Level: Intermediate
    - [React Calculator]({{site.baseurl}}/react-calculator)

### NodeJS
- Commandline:
    - [Node Quiz's app]({{site.baseurl}}/node-quizApp) -->
