# Weekly challenges for Xteam members

## Motivation
This programm is founded with the aim to train Xteam members' coding skills. Everyone in the team can contribute, by:
- Pull request your own solution (if you're really proud of it)
- Pull request new challenges. Your challenge could be from any coding languages, ranged from all levels.

### Developer's note:
- [By Minh Duc]({{site.baseurl}}/developerNote)

## Challenges included
### ReactJS
<ul>
    {% for challenge in site.reactjs %}
        <li>
            <a href="{{ challenge.url | prepend: site.baseurl }}">{{ challenge.title }}</a>
            <ul>
                <li>Level: {{challenge.level}}</li>
            </ul>
        </li>
    {% endfor %}
</ul>

### NodeJS
<ul>
    {% for challenge in site.nodejs %}
        <li>
            <a href="{{ challenge.url | prepend: site.baseurl }}">{{ challenge.title }}</a>
            <ul>
                <li>Level: {{challenge.level}}</li>
            </ul>
        </li>
    {% endfor %}
</ul>

### Other technology
<ul>
    {% for challenge in site.other %}
        <li>
            <a href="{{ challenge.url | prepend: site.baseurl }}">{{ challenge.title }}</a>
            <ul>
                <li>Level: {{challenge.level}}</li>
            </ul>
        </li>
    {% endfor %}
</ul>
