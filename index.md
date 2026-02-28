---
layout: default
---

<div class="container">
    <div class="sidebar">
        <h3>カテゴリー</h3>
        <ul>
            <li><a href="category/dokukai/index.html">読解</a><span> - 古典の言葉にふれ、人間を理解する</span></li>
            <li><a href="category/senryaku/index.html">戦略</a><span> - 歴史に学び、戦略的思考を磨く</span></li>
            <li><a href="category/shuyo/index.html">修養</a><span> - 心と体を調え、己を成長させる</span></li>
            <li><a href="category/jodo/index.html">情動</a><span> - 物語から心を動かし、共感を育む</span></li>
            <li><a href="category/daha/index.html">打破</a><span> - 過去の知恵で、現状を打破する</span></li>
        </ul>
    </div>

    <div class="main-content">
        <div class="news-area">
            <h2>新着記事</h2>
            {% for post in site.posts %}
                <div style="margin-bottom: 20px; padding: 15px; border-bottom: 1px solid #eee; background-color: #fff; border-radius: 5px;">
                    <h3 style="margin: 0 0 5px 0;"><a href="{{ site.baseurl }}{{ post.url }}" style="color: #333; text-decoration: none;">{{ post.title }}</a></h3>
                    <p style="margin: 0; font-size: 0.9em; color: #666;">{{ post.date | date: "%Y/%m/%d" }}</p>
                </div>
            {% endfor %}
        </div>
    </div>
</div>
