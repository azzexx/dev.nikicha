 <!-- Website Protect -->
<style type="text/css">
  img {
    -webkit-touch-callout:none;
    -webkit-user-select:none;
  }
</style>
  
<script id="wpcp_disable_Right_Click" type="text/javascript">
  document.ondragstart = function() { return false;}
      function nocontext(e) {
         return false;
      }
      document.oncontextmenu = nocontext;

window.addEventListener("keydown",function(e){
    if(e.ctrlKey&&(e.which==65||e.which==66||e.which==67||e.which==70||e.which==73||e.which==80||e.which==83||e.which==85||e.which==86))      {e.preventDefault()}
});
document.keypress=function(e){
    if(e.ctrlKey&&(e.which==65||e.which==66||e.which==70||e.which==67||e.which==73||e.which==80||e.which==83||e.which==85||e.which==86)){}
    return false;
}

document.onkeydown=function(e){
    e=e||window.event;
    if(e.keyCode==123||e.keyCode==18){return false}
}

       document.onclick = hideMenu; 
       document.oncontextmenu = rightClick; 

        function hideMenu() { 
            document.getElementById("contextMenu") 
                    .style.display = "none" 
        } 

        function rightClick(e) { 
            e.preventDefault(); 

            if (document.getElementById("contextMenu") .style.display == "block"){ 
                hideMenu(); 
            }else{ 
                var menu = document.getElementById("contextMenu")      
                menu.style.display = 'block'; 
                menu.style.left = e.pageX + "px"; 
                menu.style.top = e.pageY + "px"; 
            } 
        } 
</script>
<!-- End Website Protect -->