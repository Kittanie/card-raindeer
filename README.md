#card-raindeer


Basic component to render card onto screen.


## installation

component

```
$ component install kitto1/card-raindeer
```

build folder for images & build.js
```
$ component build -c
```

## usage

You can assign a custom file path for the card images if you are not working on the top layer where build lives. If you are then leave blank. 

 Use in forms/buttons or what ever else with the use of suit/num ID's. Below is a code example of Jquery for the form use of card-raindeer. 

```jquery

    var Factory = require("card-raindeer")
    var raindeer = Factory("build/")
    

      $('#button').click(function(){


        var suit = $('#suitList').val()

        var num = $('#numList').val()
        
        var src = Factory(suit,num)

        $('#img').attr('src', src)


      })
```