<h2>Shop Billing</h2>

Product: <input id="product"><br><br>
Price: <input id="price"><br><br>
Quantity: <input id="qty"><br><br>

<button onclick="bill()">Calculate Bill</button>
<button onclick="printBill()">Print Bill</button>

<h3 id="result"></h3>

<script>
function bill(){
 let p = document.getElementById("price").value;
 let q = document.getElementById("qty").value;
 let total = p*q;
 document.getElementById("result").innerHTML =
 "Total Bill = " + total;
}

function printBill(){
 window.print();
}
</script>
