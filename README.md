<div class="nav_i_public" id="nav_mouse">
	<span class="on_nav_i"  id="tab1" >导航1</span>
  <span id="tab2">导航2</span>
  <span id="tab3">导航3</span>
</div>
<div class="fu">
  <div class="text_i tab1">1</div>
  <div class="text_i hide tab2">2</div>
  <div class="text_i hide tab3">3</div>
</div>
<script type="text/javascript">
	$(document).ready(function() {		
			$("#nav_mouse span").mouseover(function(){
					$(this).addClass("on_nav_i").siblings().removeClass();			
					$(this).parent().next().children(".text_i").hide();						
					$("." + $(this).attr("id")).show();
				});  				
				$("#nav_click span").click(function(){
					$(this).addClass("on_nav_i").siblings().removeClass();			
					$(this).parent().next().children(".text_i").hide();						
					$("." + $(this).attr("id")).show();
				});    
  });
</script>
