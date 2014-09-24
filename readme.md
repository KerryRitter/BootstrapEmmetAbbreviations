#Bootstrap Emmet Abbreviations
These snippets will allow a developer to quickly generate Bootstrap components using Emmet.

##Sublime Text 3 config
1. Copy the content in "Preferences > Package Settings > Emmet > Settings - Default" to "Preferences > Package Settings > Emmet > Settings - User"
2. Copy the .json contents into the .snippets.html.abbreviations property, like so:
	"snippets": {
		"html": {
			"abbreviations": {
				"bs:dropdown": ".dropdown>button#dropdown-menu-1.btn.btn-default.dropdown-toggle[type=\"button\" data-toggle=\"dropdown\"]>span.caret^ul.dropdown-menu[role=\"menu\" aria-labelledby=\"dropdown-menu-1\"]>li[role=\"presentation\"]>a[role=\"menuitem\" tabindex=\"-1\" href=\"#\"]^+li[role=\"presentation\"].divider",
				"bs:btn-group": ".btn-group>button.btn.btn-default[type=\"button\"]*3",
				... etc ...
			}
		}
	},

##Abbreviations
###bs:dropdown
<div class="dropdown">
	<button id="dropdown-menu-1" class="btn btn-default dropdown-toggle" type="button" data-toggle="dropdown"><span class="caret"></span></button>
	<ul class="dropdown-menu" role="menu" aria-labelledby="dropdown-menu-1">
		<li role="presentation"><a href="#" role="menuitem" tabindex="-1"></a></li>
		<li role="presentation" class="divider"></li>
	</ul>
</div>

###bs:btn-group
<div class="btn-group">
	<button class="btn btn-default" type="button"></button>
	<button class="btn btn-default" type="button"></button>
	<button class="btn btn-default" type="button"></button>
</div>

###bs:input-group
<div class="input-group"><span class="input-group-addon"></span><input type="text" class="form-control"></div>

###bs:checkbox-input
<div class="input-group"><span class="input-group-addon"><input type="checkbox"></span><input type="text" class="form-control"></div>

###bs:nav-tabs
<ul class="nav nav-tabs" role="tablist">
	<li class="active"><a href=""></a></li>
	<li><a href=""></a></li>
	<li><a href=""></a></li>
</ul>

###bs:carousel
<div class="carousel slide" id="carousel-example">
	<ol class="carousel-indicators">
		<li data-target="#carousel-example" data-slide-to="1"></li>
		<li data-target="#carousel-example" data-slide-to="2"></li>
		<li data-target="#carousel-example" data-slide-to="3"></li>
	</ol>
	<div class="carousel-inner">
		<div class="item">
			<img src="http://lorempixel.com/1170/300" alt="Image">
			<div class="carousel-caption">This is a caption 1</div>
		</div>
		<div class="item">
			<img src="http://lorempixel.com/1170/300" alt="Image">
			<div class="carousel-caption">This is a caption 2</div>
		</div>
		<div class="item">
			<img src="http://lorempixel.com/1170/300" alt="Image">
			<div class="carousel-caption">This is a caption 3</div>
		</div>
	</div>
	<a href="carousel-example" data-slide="prev" class="left carousel-control"><span class="icon-prev"></span></a>
	<a href="carousel-example" data-slide="next" class="right carousel-control"><span class="icon-next"></span></a>
</div>

###bs:navbar
<div class="navbar navbar-default navbar-fixed">
	<div class="container">
		<div class="navbar-header">
			<div class="navbar-brand"></div>
			<button class="navbar-toggled collapsed" type="button" data-toggle="collapse" data-target="#main-menu">
				<span class="icon-bar"></span>
				<span class="icon-bar"></span>
				<span class="icon-bar"></span></button>
		</div>
		<div class="navbar-collapse collapse">
			<div id="main-menu" class="navbar-collapse">
				<ul class="nav navbar-nav">
					<li><a href=""></a></li>
					<li><a href=""></a></li>
					<li><a href=""></a></li>
				</ul>
			</div>
		</div>
	</div>
</div>

###bs:panel
<div class="panel panel-deafult">
	<div class="panel-heading">
		<h3 class="panel-title"></h3>
	</div>
	<div class="panel-body"></div>
	<div class="panel-footer"></div>
</div>

###.jumbotron>.container>h1+p+p>a.btn-btn.primary.btn-lg
<div class="jumbotron">
	<div class="container">
		<h1></h1>
		<p></p>
		<p><a href="" class="btn-btn primary btn-lg"></a></p>
	</div>
</div>

###bs:page-header
<div class="page-header">
	<h1></h1>
</div>

###bs:thumbnail
<div class="thumbnail">
	<img src="" alt="">
	<div class="caption">
		<h3></h3>
		<p></p>
		<p><a href="" class="btn btn-primary"></a></p>
	</div>
</div>

###bs:thumbnail
<div class="thumbnail">
	<img src="" alt="">
	<div class="caption">
		<h3></h3>
		<p></p>
		<p><a href="" class="btn btn-primary"></a></p>
	</div>
</div>

###bs:alert
<div class="alert" role="alert">
	<p><strong></strong><span></span></p>
</div>

###bs:grid12
<div class="row">
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
	<div class="col-xs-1"></div>
</div>

###bs:grid6
<div class="row">
	<div class="col-xs-2"></div>
	<div class="col-xs-2"></div>
	<div class="col-xs-2"></div>
	<div class="col-xs-2"></div>
	<div class="col-xs-2"></div>
	<div class="col-xs-2"></div>
</div>

###bs:grid4
<div class="row">
	<div class="col-xs-3"></div>
	<div class="col-xs-3"></div>
	<div class="col-xs-3"></div>
	<div class="col-xs-3"></div>
</div>

###bs:grid3
<div class="row">
	<div class="col-xs-4"></div>
	<div class="col-xs-4"></div>
	<div class="col-xs-4"></div>
</div>

###bs:grid2
<div class="row">
	<div class="col-xs-6"></div>
	<div class="col-xs-6"></div>
</div>