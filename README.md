# SIGNAL Lab Website


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
在data目录中team_en.yaml以及team_zh.yaml添加个人信息即可，格式如下：
```yaml
- name: 名字
  photo: 照片
  info: 职称
  email: 邮箱
  biography: 个人简介
  position: 身份，可选director、member、phd、master
  interests: 研究兴趣，只有phd和master需要
```
其中照片文件应该放置在static/team目录中。

### Add news
在data目录中news_en.yaml以及news_zh.yaml中添加新闻即可，格式如下：
```yaml
- title: 新闻标题（支持在其中使用html标签）
  date: 发布日期
  icon: 一个Emoji图标（可选）
  author: 作者
  detail: 详情（可选，支持在其中使用html标签）
```

**注意**：每次添加新闻总应该添加在数据文件的最上方

### Add seminae
在content/seminars中创建一个新的文件夹，然后在其中添加index.en.md和index.zh-cn.md（可以只添加一个语言版本）具体格式参考content/seminars/basic-markdown-syntax。

### 维护首页
#### 修改文字内容
直接编辑content/_index.en.md和content/_index.zh-cn.md文件即可。

#### 修改轮播图
首先将需要的图片放置在static/slide目录中，然后编辑data/slide.yaml指定想要轮播展示的图片的文件名，这里图片的个数不受限制。

#### 修改Quick Links
编辑data目录中quick_link_en.yaml和quick_link_zh.yaml即可，格式如下：
```yaml
- title: 超链接文本
  link: 链接地址
```

