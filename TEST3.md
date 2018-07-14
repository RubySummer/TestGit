    class A{
         if(i<0){
           int b =5;
           System.out.println("kkk");
         }
     }
<pre class="prettyprint lang-javascript">  
function getNowDate() {
    var date = new Date();
    var split = "-";
    var year = date.getFullYear();
    var month = date.getMonth() + 1;
    var strDate = date.getDate();
    if (month >= 1 && month <= 9) {
        month = "0" + month;
    }
    if (strDate >= 0 && strDate <= 9) {
        strDate = "0" + strDate;
    }
    var currentdate = year + split + month + split + strDate;
    return currentdate;
}
</pre> 
