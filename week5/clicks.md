###Capturing Clicks!

---

Let's do something when our user clicks using JQuery! Add a `<script>` tag at the bottom of your `<body`

```
<script>
$(document).ready(function(){
    
    $("#jellyfish").click(function(){
        $("#jellyfish").append( "<i class='em em-octopus'></i>");
    });

    $("#turtle").click(function(){
        $(".em-turtle").last().remove();
    });

    $("#ice").click(function(){
        $(".em-icecream").last().remove();    
    });
    
});

</script>
```
