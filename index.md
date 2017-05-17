
---
layout: post
title: Mathematical scribblings

---

<div class="page-header">
  <h1>
    {{ site.author.name }}
    {% if site.tagline %}<br/><small>{{ site.tagline }}</small>{% endif %}
  </h1>
</div>

<!-- recent posts -->
<div id="recent-posts" class="recent-posts">
  {% for this_post in paginator.posts %}
  <div class="post">
      <a href="{{ this_post.url }}">
        <h2 class="post-title">{{ this_post.title }}</h2>
      </a>
      {% include category_info %}
      {% include source_info %}
      <div class="post-content">
          {{ this_post.excerpt }}
      </div>
      <div class="align-right">
        <a href="{{ this_post.url }}">more ...</a>
      </div>
  </div>
  {% endfor %}
</div>
<script type="text/javascript">
  var el = document.getElementById("recent-posts");
  fix_cjk_linebreak(el);
  fix_table_style(el);
</script>

<!-- pagination links -->
<div class="pagination align-center">
  <ul class="pagination">
    {% if paginator.next_page %}
    <li class="prev">
      <a href="{{ paginator.next_page_path }}">&laquo; Older</a>
    </li>
    {% else %}
    <li class="prev disabled">
      <a>&laquo; Older</a>
    </li>
    {% endif %}
    <li>
      <a href="{{ BASE_PATH }}{{ site.JB.archive_path }}">Archive</a>
    </li>
    {% if paginator.previous_page %}
    <li class="next">
      {% if paginator.previous_page == 1 %}
      <a href="/">Newer &raquo;</a>
      {% else %}
      <a href="{{ paginator.previous_page_path }}">Newer &raquo;</a>
      {% endif %}
    </li>
    {% else %}
    <li class="next disabled">
      <a>Newer &raquo;</a>
    </li>
    {% endif %}
  </ul>
</div>















# CARGO notes #





# Research #





# Philosophy of mathematics #
[Topos, being, and existence][TBE]



# Recreational mathematics 



[TBE]: 2017-05-17-Topos-being-and-existence.html
