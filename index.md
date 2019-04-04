# Weekly challenges for Xteam members

## Motivation
This programm is founded with the aim to train Xteam members' coding skills. Everyone in the team can contribute, by:
- Pull request your own solution (if you're really proud of it)
- Pull request new challenges. Your challenge could be from any coding languages, ranged from all levels.

## Developer's note:
- [By Minh Duc]({{site.baseurl}}/developerNote)

## Rules :)
```json
{"XTEAM CODING CHALLENGE PROGRAMM": 
  {
    "CÓ BẮT BUỘC KHÔNG": true,
    "THỜI GIAN ĐĂNG CHALLENGE MỖI TUẦN": "T5 hàng tuần",
    "NỘI DUNG CHALLENGE": "Theo hứng của tớ :> || Theo đề xuất của mọi người",
    "CÁCH DEPLOY CODE ĐỐI VỚI": {
        "NodeJS": ["Link Github", "Link RePL"],
        "ReactJS (hoặc các Frontend Project khác)": ["Link Github", "Link CodeSandBox", "Link CodePen"],
        "Những Project khác": "Tính sau"
    },
    "CÁCH NỘP BÀI": "CMT LINK BÀI TRÊN POST ĐĂNG CHALLENGE",
    "HÌNH THỨC THEO DÕI": "Qua sheet Google (pin trên gr Facebook)",
    "CÁC TRƯỜNG HỢP BỊ TICK": {
        "THÀNH VIÊN": {
            "CHẬM NỘP BÀI && KHÔNG BÁO TRƯỚC": "1 TICK"
        },
        "TRƯỞNG BAN": {
            "CHẬM ĐĂNG CHALLENGE": "2 TICK"
        }
    }
  }
}
```

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
