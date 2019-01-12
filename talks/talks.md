<h3 class="masthead-title">
<!-- <a href="/" title="Home">{{ site.title }}</a> -->
<a href="/" title="Home">Home</a>

{% for page in site.pages_list %}
  &nbsp;&nbsp;&nbsp;
  <a href="{{ page[1]  }}">{{ page[0] }}</a>
{% endfor %}
</h3>

Robotics: Science and Systems (RSS) Conference - June 27, 2018

<iframe width="560" height="315" src="https://www.youtube.com/embed/mBEhcmhvUdA?start=2904" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<body>

	<div id="loginbox" class="lightbox" >
		<div class="horizontal">
			<div class="vertical">
				<div class="box">
					<input style="margin: 16px; text-align: center;" id="password" type="password" placeholder="password" /> <br />
					<button id="loginbutton" type="button">Enter</button>
					<p id="wrongPassword" style="display: none">wrong password</p>
				</div>
			</div>
		</div>
	</div>



	<script type="text/javascript" src="https://code.jquery.com/jquery-1.12.0.min.js"></script>


	 <script type="text/javascript" src="https://rawcdn.githack.com/chrisveness/crypto/7067ee62f18c76dd4a9d372a00e647205460b62b/sha1.js"></script>

	<script type="text/javascript">
	"use strict";
	function loadPage(pwd) {
		var hash= pwd;
		hash= Sha1.hash(pwd);
		var url= hash + "/index.html";
		$.ajax({
			url : url,
			dataType : "html",
			success : function(data) {
				window.location= url;
			},
			error : function(xhr, ajaxOptions, thrownError) {
				parent.location.hash= hash;
				//$("#wrongPassword").show();
				$("#password").attr("placeholder","wrong password");
				$("#password").val("");
			}
		});
	}
	$("#loginbutton").on("click", function() {
		loadPage($("#password").val());
	});
	$("#password").keypress(function(e) {
		if (e.which == 13) {
			loadPage($("#password").val());
		}
	});
	$("#password").focus();
	</script>

</body>
