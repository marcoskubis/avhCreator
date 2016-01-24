# avhCreator
PHP Apache Virtual Host Creator for WAMP

### Configuration

The first thing to do is config only three varables:

- The wamp's www path.
<pre>
$www_dir = 'C:/wamp/www/';
</pre>

- The `httpd-vhosts.conf` file location. Here, almost in all of the cases the only thing that changes is the version of apache.
<pre>
$httpdVhosts = 'C:\wamp\bin\apache\apache2.4.9\conf\extra\httpd-vhosts.conf';
</pre>

- The apache service name. This might be `wampapache64` for 64 bits machines, or `wampapache` for 32 bits.
<pre>
$apache_service_name = 'wampapache64';
</pre>

### Running
First, download the `avhCreator` file from this repository.<br />
Open terminal as Administrator and run this command:
<pre>
cd /location/of/avhCreator/file
php avhCreator &ltserverName&gt &ltpublicFolder&gt
</pre>
#### Parameters
<table>
	<tr>
		<th>Parameter</th>
		<th>Required</th>
		<th>Default value</th>
		<th>Description</th>
	</tr>
	<tr>
		<td>serverName</td>
		<td>yes</td>
		<td></td>
		<td>The name of the server that you want create.<br /><small>Ex.: myecommerce.app, myblog.app, ...</small></td>
	</tr>
	<tr>
		<td>publicFolder</td>
		<td>no</td>
		<td>public</td>
		<td>The public folder for your server.<br /><small>Ex.: public, public_html, web, ...</small></td>
	</tr>
</table>
#### Example
<pre>
php avhCreator myblog.app public_html
</pre>
And then, go to http://myblog.app
