# SIGNAL Lab Website

Revised from [link](https://github.com/csl-cqu/csl-cqu.github.io)

### Add Publication
```yaml
- title: "paper title"
  highlight: e.g. "Best Paper", "Oral", "Spotlight"
  authors: authors
  publication: journal/conference
  link: url for publication
```

It is worth noting that if you need to add a year, you need to create the publicationsxxxx.yaml file corresponding to the year in the data directory, and then edit `layouts/shortcodes/publications-en.html` and `layouts/shortcodes/publications-zh.html `, just add the corresponding content. For example, if you add 2023, add the following content above `<h2 id="2022">2022</h2>`

```html
<h2 id="2023">2023</h2>
<ul>
    {{ range .Site.Data.publications2023 }}
        <li>
            <p><b><a href="{{ .link }}">{{ .title }}
                {{ if .highlight }}
                <span style="color: red;">
                    ({{ .highlight }})
                </span>
                {{ end }}
            </a></b></p>
            <p>{{.authors}}</p>
            <p><i>{{.publication}}</i>
                {{ if .ccf_rank }}
                , <b>CCF Rank {{.ccf_rank}}</b>
                {{ end }}
                {{ if .cqu_rank }}
                , <b>CSL@CQU Rank {{.cqu_rank}}</b>
                {{ end }}
            </p>
        </li>
    {{ end }}
</ul>
```

### Add Team Member
add to data/team_en.yaml, see the following form：
```yaml
- name: 
  photo: 
  info: 
  email:
  biography:
  position: member、phd、master
  interests: 
```
photo is saved in static/team

p.s. master means master+undergrad. member means visiting student

### Add news
add to data/news_en.yaml，from：
```yaml
- title: 
  date:
  icon:one Emoji图标
  author: 
  detail: use html
```

**Notice**：new news should be added to the top

### Add seminar
creat a new folder in content/seminars，then adde index.en.md to the folder. examples see content/seminars/basic-markdown-syntax。

### Others
#### Home page
edit content/_index.en.md


#### Quick Links
data/quick_link_en.yaml
```yaml
- title: 
  link: 
```

