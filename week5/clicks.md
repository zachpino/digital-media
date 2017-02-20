###Capturing Clicks!

---


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

    $("#system-ul").hover(function(){
    	$("#more-info").text("Part 1 of my system")
    },
    function(){
		$("#more-info").text("The major parts of the platform...")
	}	
    );

    $("#system-um").hover(function(){
    	$("#more-info").text("Part 2 of my system")
    },
    function(){
		$("#more-info").text("The major parts of the platform...")
	}	
    );

    $("#system-ur").hover(function(){
    	$("#more-info").text("Part 3 of my system")
    },
    function(){
		$("#more-info").text("The major parts of the platform...")
	}	
    );

    $(".storyboard-image").click(function(){
        var image = $(this).attr("src");
           

        $("#hero-image").animate({"opacity":0}, 1500, function(){$("#hero-image").attr('src', image);});

        $("#hero-image").animate({"opacity":1}, 1500 );
    });

});

</script>
```
