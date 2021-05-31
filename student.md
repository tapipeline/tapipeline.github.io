<style>
  p {margin-right: auto;}
  img {margin-left: auto;}
</style>
<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      

      <div class="entry">
        <img src="{{ post.image }}">
        <p><h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1><p>
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
