{% highlight javascript %}

    var MyApp = {};
    (function() {

      this.photoRemovalPrompt = function() {
        $('a.remove-photo').click(function(ev) { 
          if (confirm('Are you sure you want to remove this photo?')) {
            $(this).parent('form').submit(); 
          }
        });
      }
    }).call(MyApp);
      
{% endhighlight %}
