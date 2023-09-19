# calculator_project

<input type="number" value="number" id="first">
           <select name="name" id="ope">
            <option value="+">+</option>
            <option value="-">-</option>
            <option value="*">x</option>
            <option value="/">/</option>
           </select>
         <input type="number" value="number" id="second">
         <br>
         <br>
         <button onclick="col()">Calculate</button>
         <input type="number" value="number" id="res" readonly>
           <script>
            function col(){
                var opr1 = document.getElementById("first").value;
                var opr2 = document.getElementById("second").value;
                var opr3 = document.getElementById("ope").value;
               if (opr3 == '+'){
                  var calc = parseInt(opr1) + parseInt(opr2);
               }
               else if ( opr3 == '-'){
                var calc = parseInt(opr1)- parseInt(opr2);
               }
               else if(opr3 == '*') {
                var calc = parseInt(opr1) * parseInt(opr2);
               }
               else if  (opr3 == '/') {
                 var calc = parseInt(opr1) / parseInt(opr2);
               }
                   document.getElementById('res').value= calc;
            }
           </script>
