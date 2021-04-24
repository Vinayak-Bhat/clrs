
## Notes on 'Introduction to Algorithms'

My notes on the book *Introduction to Algorithms* by Thomas H. Cormen, Charles E. Leiserson, Ronald Rivest, Clifford Stein.

Here is an aside, which I did not know until I wrote this page: <https://www.writersdigest.com/whats-new/do-you-underline-book-titles>


<ul>
  {% for page in site.pages %}
   

       {% if page.page == true %}
          <li><a href="{{ page.url }}">{{ page.title }}</a></li>
    
         {% endif %} 
  {% endfor %}  <!-- page -->
</ul>
