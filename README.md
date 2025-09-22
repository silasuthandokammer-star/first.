
 <!DOCTYPE html>
<html>
    <head>
        <title>Coffee Shop</title>
    </head>

<body>
    <p>Hello, how are you doing?</p>
    <p id="demo"></p>

    <button id="coffe1">latte</button>
     <p id="balance">balance: 10FC</p>

    <script>
        let balance = 10;
        let coffePrice = 4;

      document.getElementById("demo").innerHTML = "what coffe would you like?";
       
    function updatebalance() {
        document.getElementById("balance").innerHTML = "balance:" + balance + "FC";
    }
     updatebalance();   
      
      document.getElementById("coffe1").onclick = function ()  { 
      if (balance >= coffePrice) {
if (confirm("your total is " + coffePrice + "FC. Confirm purchase"))  {
    balance -= coffePrice;
    updatebalance();
     alert("Thanks for your purchase");
} else {alert("fuck you")}
    
       
      }
      }
      
    


    </script>

</body>
</html>
