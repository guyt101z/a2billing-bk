<!-- 
	Index template for the A2billing customer login screen. This file should overwrite file located at 
	/var/www/html/a2billing/customer/templates/default/index.tpl
	Notice that this files links to external content (twitter github). Make sure you can link to external sites in you server.
	For install intructions please check devaleph.com/blog
	Created by Ulises on 05Nov2012 - Contact: ulises at devaleph dot com	
	
	This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-->
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
		<meta charset="utf-8">
		<link rel="shortcut icon" href="templates/{$SKIN_NAME}/images/favicon.ico">
		<title>..:: {$CCMAINTITLE} ::..</title>
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		<meta name="description" content="">
		<meta name="author" content="">
		<!-- Le styles -->
		<link href="http://twitter.github.com/bootstrap/assets/css/bootstrap.css" rel="stylesheet">
		<link href="http://twitter.github.com/bootstrap/assets/css/bootstrap-responsive.css" rel="stylesheet">
		<script type="text/javascript" src="./javascript/jquery/jquery-1.2.6.min.js"></script>
		<!-- Le HTML5 shim, for IE6-8 support of HTML5 elements -->
		<!--[if lt IE 9]>
		<script src="http://html5shim.googlecode.com/svn/trunk/html5.js"></script>
		<![endif]-->
	</head>
	<body>
		<script LANGUAGE="JavaScript">
			{literal}
			function test()
			{
			if(document.form.pr_login.value=="" || document.form.pr_password.value=="")
			{
			alert("You must enter an user and a password!" + document.form.pr_password.value);
			return false;
			}
			else
			{
			return true;
			}
			}
			{/literal}
		</script>
		<div class="navbar navbar-inverse navbar-fixed-top">
			<div class="navbar-inner">
				<div class="container">
					<a class="brand" href="index.php">{$CCMAINTITLE}</a>
				</div>
			</div>
		</div>
		<form name="form" method="POST" action="userinfo.php" onsubmit="return test()" class="form-horizontal">
			<input type="hidden" name="done" value="submit_log">
			<div class="container">
				<div class="hero-unit">
					<h1>{php} echo gettext("AUTHENTICATION");{/php}</h1>
				</div>
				{if ($error == 1)}
				<div class="alert alert-error">
					{php} echo gettext("AUTHENTICATION REFUSED, please check your user/password!");{/php}
				</DIV>
				{elseif ($error==2)}
				<div class="alert alert-error">
					{php} echo gettext("INACTIVE ACCOUNT, Please activate your account!");{/php}
				</div>
				{elseif ($error==3)}
				<div class="alert alert-error">
					{php} echo gettext("BLOCKED ACCOUNT, Please contact the administrator!");{/php}
				</div>
				{/if}
					<div class="control-group">
						<label class="control-label" for="inputEmail">{php} echo gettext("User");{/php}:</label>
						<div class="controls">
							<input type="text" name="pr_login" id="pr_login" placeholder="{$username}" value="{$username}">
						</div>
					</div>
					<div class="control-group">
						<label class="control-label" for="inputPassword">{php} echo gettext("Password");{/php}:</label>
						<div class="controls">
							<input type="password" id="pr_password" name="pr_password" placeholder="{$password}" value="{$password}">
						</div>
					</div>
					<div class="control-group">
						<label class="control-label" for="inputPassword"></label>
						<div class="controls">
							<select name="ui_language" id="ui_language" >
								    <option style="background:url(templates/{$SKIN_NAME}/images/flags/gb.gif) no-repeat left center;padding-left:25px;" value="english" {php} if(LANGUAGE=="english") echo "selected";{/php} >English</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/es.gif) no-repeat left center;padding-left:25px;" value="spanish" {php} if(LANGUAGE=="spanish") echo "selected";{/php} >Spanish</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/fr.gif) no-repeat left center;padding-left:25px;" value="french" {php} if(LANGUAGE=="french") echo "selected";{/php} >French</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/de.gif) no-repeat left center;padding-left:25px;" value="german" {php} if(LANGUAGE=="german") echo "selected";{/php} >German</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/pt.gif) no-repeat left center;padding-left:25px;" value="portuguese" {php} if(LANGUAGE=="portuguese") echo "selected";{/php} >Portuguese</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/br.gif) no-repeat left center;padding-left:25px;" value="brazilian" {php} if(LANGUAGE=="brazilian") echo "selected";{/php}>Brazilian</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/it.gif) no-repeat left center;padding-left:25px;" value="italian" {php} if(LANGUAGE=="italian") echo "selected";{/php} >Italian</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/cn.gif) no-repeat left center;padding-left:25px;" value="chinese" {php} if(LANGUAGE=="chinese") echo "selected";{/php} >Chinese</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/ro.gif) no-repeat left center;padding-left:25px;" value="romanian" {php} if(LANGUAGE=="romanian") echo "selected";{/php} >Romanian</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/pl.gif) no-repeat left center;padding-left:25px;" value="polish" {php} if(LANGUAGE=="polish") echo "selected";{/php} >Polish</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/ru.gif) no-repeat left center;padding-left:25px;" value="russian" {php} if(LANGUAGE=="russian") echo "selected";{/php} >Russian</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/tr.gif) no-repeat left center;padding-left:25px;" value="turkish" {php} if(LANGUAGE=="turkish") echo "selected";{/php} >Turkish</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/pk.gif) no-repeat left center;padding-left:25px;" value="urdu" {php} if(LANGUAGE=="urdu") echo "selected";{/php} >Urdu</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/ua.gif) no-repeat left center;padding-left:25px;" value="ukrainian" {php} if(LANGUAGE=="ukrainian") echo "selected";{/php} >Ukrainian</option>
			                        <option style="background:url(templates/{$SKIN_NAME}/images/flags/gr.gif) no-repeat left center;padding-left:25px;" value="greek" {php} if(LANGUAGE=="greek") echo "selected";{/php} >Greek</option>
							</select>
						</div>
					</div>
					<div class="control-group">
						<div class="controls">
							<button type="submit" class="btn btn-large btn-success" id="submit" name="submit" style="width: 220px;">
								{php} echo gettext("LOGIN");{/php}
							</button>
						</div>
					</div>
					<div class="well">
						{php} echo gettext("Forgot your password ?");{/php} <a href="forgotpassword.php"><span class="label label-important">{php} echo gettext("Click here");{/php}</span></a>
					</div>	
					<div class="well">
						{php} echo gettext("To sign up");{/php} <a href="signup.php"><span class="label label-info">{php} echo gettext("Click here");{/php}</span></a></a>
					</div>
					<hr>
					<footer>
						<p>
							<div class="container">{$COPYRIGHT}</div>
						</p>
					</footer>
			</div>
		</div>
		</form>
		{literal}
		<script LANGUAGE="JavaScript">
			//document.form.pr_login.focus();
			$("#ui_language").change(function() {
				self.location.href = "index.php?ui_language=" + $("#ui_language option:selected").val();
			});

		</script>
		{/literal}
