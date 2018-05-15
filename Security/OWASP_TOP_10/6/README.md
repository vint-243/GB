<html>
<head>
<META http-equiv="Content-Type" content="text/html; charset=UTF-8">
<title>ZAP Scanning Report</title>
<style>
body{
  font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
  color: #000;
  font-size: 13px;
}
h1{
  text-align: center;
  font-weight: bold;
  font-size: 32px
}
h3{
  font-size: 16px;
}
table{
  border: none;
  font-size: 13px;
}
td, th {
  padding: 3px 4px;
}
th{
  font-weight: bold;
}
.results th{
  text-align: left;
}
.spacer{
  margin: 10px;
}
.spacer-lg{
  margin: 40px;
}
.indent1{
  padding: 4px 20px;
}
.indent2{
  padding: 4px 40px;
}
.risk-high{
  background-color: red;
  color: #FFF;
}
.risk-medium{
  background-color: orange;
  color: #FFF;
}
.risk-low{
  background-color: yellow;
  color: #000;
}
.risk-info{
  background-color: blue;
  color: #FFF;
}
.summary th{
  color: #FFF;
}
</style>
</head>
<body>
<h1>
<img src="data:image/png;base64,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">
ZAP Scanning Report
</h1>
<p>

</p>
<h3>Summary of Alerts</h3>
<table width="45%" class="summary">
<tr bgcolor="#666666">
<th width="45%" height="24">Risk 
      Level</th><th width="55%" align="center">Number 
      of Alerts</th>
</tr>
<tr bgcolor="#e8e8e8">
<td><a href="#high">High</a></td><td align="center">5</td>
</tr>
<tr bgcolor="#e8e8e8">
<td><a href="#medium">Medium</a></td><td align="center">7</td>
</tr>
<tr bgcolor="#e8e8e8">
<td><a href="#low">Low</a></td><td align="center">10</td>
</tr>
<tr bgcolor="#e8e8e8">
<td><a href="#info">Informational</a></td><td align="center">10</td>
</tr>
</table>
<div class="spacer-lg"></div>
<h3>Alert Detail</h3>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-high">
<th width="20%"><a name="high"></a>High (Medium)</th><th width="80%">Insecure Component - Apache 2.2.8</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Based on passive analysis of the response, insecure component Apache 2.2.8 appears to be in use.</p><p>The highest noted CVSS rating for this product version is 10.</p><p>In total, 31 vulnerabilities were noted.</p><p>Some Linux distributions such as Red Hat employ the practice of retaining old version numbers when security fixes are "backported".</p><p>These cases are noted as "False Positives", but should be manually verified.  </p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">Apache/2.2.8 (Ubuntu) DAV/2</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">Apache/2.2.8 (Ubuntu) DAV/2</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/html5.js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">Apache/2.2.8 (Ubuntu) DAV/2</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/stylesheet.css</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">Apache/2.2.8 (Ubuntu) DAV/2</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">4</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Upgrade from Apache 2.2.8 to the latest stable version of the product.</p><p>Use a package manager and package management policies and procedures to manage the installed versions of software packages.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>CVE: CVE-2010-0425</p><p>CVSS: 10.0</p><p></p><p>CVE: CVE-2011-3192</p><p>CVSS: 7.8</p><p></p><p>CVE: CVE-2013-2249</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2009-1890</p><p>CVSS: 7.1</p><p></p><p>CVE: CVE-2009-1891</p><p>CVSS: 7.1</p><p></p><p>CVE: CVE-2012-0883</p><p>CVSS: 6.9</p><p></p><p>CVE: CVE-2009-3555</p><p>CVSS: 5.8</p><p></p><p>CVE: CVE-2013-1862</p><p>CVSS: 5.1</p><p></p><p>CVE: CVE-2007-6750</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2008-2364</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2009-2699</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-0408</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-1452</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2011-3368</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2013-6438</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2014-0098</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2009-1195</p><p>CVSS: 4.9</p><p></p><p>CVE: CVE-2012-0031</p><p>CVSS: 4.6</p><p></p><p>CVE: CVE-2011-3607</p><p>CVSS: 4.4</p><p></p><p>CVE: CVE-2008-2939</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2010-0434</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2011-0419</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2011-3348</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2011-3639</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2011-4317</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2012-0053</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2012-3499</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2012-4558</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2013-1896</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2012-2687</p><p>CVSS: 2.6</p><p></p><p>CVE: CVE-2011-4415</p><p>CVSS: 1.2</p><p></p><p></p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-0425</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-3192</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2013-2249</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-1890</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-1891</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-0883</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-3555</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2013-1862</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-6750</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-2364</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-2699</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-0408</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1452</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-3368</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2013-6438</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2014-0098</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-1195</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-0031</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-3607</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-2939</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-0434</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-0419</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-3348</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-3639</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-4317</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-0053</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-3499</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-4558</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2013-1896</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-2687</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-4415</p><p></p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">829</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">42</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-high">
<th width="20%"><a name="high"></a>High (Medium)</th><th width="80%">Anti CSRF Tokens Scanner</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>A cross-site request forgery is an attack that involves forcing a victim to send an HTTP request to a target destination without their knowledge or intent in order to perform an action as the victim. The underlying cause is application functionality using predictable URL/form actions in a repeatable way. The nature of the attack is that CSRF exploits the trust that a web site has for a user. By contrast, cross-site scripting (XSS) exploits the trust that a user has for a web site. Like XSS, CSRF attacks are not necessarily cross-site, but they can be. Cross-site request forgery is also known as CSRF, XSRF, one-click attack, session riding, confused deputy, and sea surf.</p><p></p><p>CSRF attacks are effective in a number of situations, including:</p><p>    * The victim has an active session on the target site.</p><p>    * The victim is authenticated via HTTP auth on the target site.</p><p>    * The victim is on the same local network as the target site.</p><p></p><p>CSRF has primarily been used to perform an action against a target site using the victim's privileges, but recent techniques have been discovered to disclose information by gaining access to the response. The risk of information disclosure is dramatically increased when the target site is vulnerable to XSS, because XSS can be used as a platform for CSRF, allowing the attack to operate within the bounds of the same-origin policy.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">&lt;form action="/bwapp/bWAPP/portal.php" method="POST"&gt;</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Phase: Architecture and Design</p><p>Use a vetted library or framework that does not allow this weakness to occur or provides constructs that make this weakness easier to avoid.</p><p>For example, use anti-CSRF packages such as the OWASP CSRFGuard.</p><p></p><p>Phase: Implementation</p><p>Ensure that your application is free of cross-site scripting issues, because most CSRF defenses can be bypassed using attacker-controlled script.</p><p></p><p>Phase: Architecture and Design</p><p>Generate a unique nonce for each form, place the nonce into the form, and verify the nonce upon receipt of the form. Be sure that the nonce is not predictable (CWE-330).</p><p>Note that this can be bypassed using XSS.</p><p></p><p>Identify especially dangerous operations. When the user performs a dangerous operation, send a separate confirmation request to ensure that the user intended to perform that operation.</p><p>Note that this can be bypassed using XSS.</p><p></p><p>Use the ESAPI Session Management control.</p><p>This control includes a component for CSRF.</p><p></p><p>Do not use the GET method for any request that triggers a state change.</p><p></p><p>Phase: Implementation</p><p>Check the HTTP Referer header to see if the request originated from an expected page. This could break legitimate functionality, because users or proxies may have disabled sending the Referer for privacy reasons.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://projects.webappsec.org/Cross-Site-Request-Forgery</p><p>http://cwe.mitre.org/data/definitions/352.html</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">352</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">9</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-high">
<th width="20%"><a name="high"></a>High (Medium)</th><th width="80%">Insecure Component - PHP 5.2.4</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Based on passive analysis of the response, insecure component PHP 5.2.4 appears to be in use.</p><p>The highest noted CVSS rating for this product version is 10.</p><p>In total, 112 vulnerabilities were noted.</p><p>Some Linux distributions such as Red Hat employ the practice of retaining old version numbers when security fixes are "backported".</p><p>These cases are noted as "False Positives", but should be manually verified.  </p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">PHP/5.2.4-2ubuntu5.10</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Upgrade from PHP 5.2.4 to the latest stable version of the product.</p><p>Use a package manager and package management policies and procedures to manage the installed versions of software packages.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>CVE: CVE-2008-0599</p><p>CVSS: 10.0</p><p></p><p>CVE: CVE-2008-2050</p><p>CVSS: 10.0</p><p></p><p>CVE: CVE-2008-2051</p><p>CVSS: 10.0</p><p></p><p>CVE: CVE-2008-5557</p><p>CVSS: 10.0</p><p></p><p>CVE: CVE-2009-4143</p><p>CVSS: 10.0</p><p></p><p>CVE: CVE-2011-3268</p><p>CVSS: 10.0</p><p></p><p>CVE: CVE-2012-2376</p><p>CVSS: 10.0</p><p></p><p>CVE: CVE-2012-2688</p><p>CVSS: 10.0</p><p></p><p>CVE: CVE-2007-1581</p><p>CVSS: 9.3</p><p></p><p>CVE: CVE-2007-5653</p><p>CVSS: 9.3</p><p></p><p>CVE: CVE-2008-2107</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2008-2108</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2008-3658</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2008-5624</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2008-5625</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2008-5658</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2009-3291</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2009-3292</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2009-3293</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2009-4018</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2010-1129</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2010-1868</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2010-2225</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2011-1092</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2011-1153</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2012-1823</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2012-2311</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2012-2386</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2013-1635</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2014-8626</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2014-9427</p><p>CVSS: 7.5</p><p></p><p>CVE: CVE-2007-5900</p><p>CVSS: 6.9</p><p></p><p>CVE: CVE-2007-4889</p><p>CVSS: 6.8</p><p></p><p>CVE: CVE-2010-3870</p><p>CVSS: 6.8</p><p></p><p>CVE: CVE-2010-4697</p><p>CVSS: 6.8</p><p></p><p>CVE: CVE-2011-4718</p><p>CVSS: 6.8</p><p></p><p>CVE: CVE-2012-0831</p><p>CVSS: 6.8</p><p></p><p>CVE: CVE-2007-5898</p><p>CVSS: 6.4</p><p></p><p>CVE: CVE-2008-3659</p><p>CVSS: 6.4</p><p></p><p>CVE: CVE-2009-2626</p><p>CVSS: 6.4</p><p></p><p>CVE: CVE-2010-1128</p><p>CVSS: 6.4</p><p></p><p>CVE: CVE-2010-1861</p><p>CVSS: 6.4</p><p></p><p>CVE: CVE-2010-2191</p><p>CVSS: 6.4</p><p></p><p>CVE: CVE-2012-0057</p><p>CVSS: 6.4</p><p></p><p>CVE: CVE-2012-1172</p><p>CVSS: 5.8</p><p></p><p>CVE: CVE-2008-4107</p><p>CVSS: 5.1</p><p></p><p>CVE: CVE-2006-7243</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2007-4783</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2007-4840</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2007-4850</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2008-2666</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2008-3660</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2008-5498</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2009-1271</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2009-1272</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2009-3294</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2009-4418</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-1130</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-1860</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-1862</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-1864</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-1914</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-1915</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-1917</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-2093</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-2097</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-2100</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-2101</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-2190</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-2484</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-3065</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-4150</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-4645</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-4698</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2010-4699</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2011-0752</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2011-0755</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2011-1466</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2011-1467</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2011-2483</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2011-3182</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2011-3267</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2011-4885</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2012-0788</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2012-0789</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2012-1171</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2012-2336</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2012-3365</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2013-1643</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2013-2110</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2013-4635</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2014-0237</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2014-0238</p><p>CVSS: 5.0</p><p></p><p>CVE: CVE-2007-4887</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2007-5447</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2007-5899</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2009-4142</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2010-2531</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2010-3709</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2010-3710</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2011-0421</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2011-0708</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2011-1464</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2011-1468</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2011-1469</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2011-1470</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2012-2143</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2013-4248</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2014-2497</p><p>CVSS: 4.3</p><p></p><p>CVE: CVE-2014-5459</p><p>CVSS: 3.6</p><p></p><p>CVE: CVE-2008-5814</p><p>CVSS: 2.6</p><p></p><p>CVE: CVE-2007-6039</p><p>CVSS: 2.1</p><p></p><p></p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-0599</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-2050</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-2051</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-5557</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-4143</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-3268</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-2376</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-2688</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-1581</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-5653</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-2107</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-2108</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-3658</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-5624</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-5625</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-5658</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-3291</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-3292</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-3293</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-4018</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1129</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1868</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-2225</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-1092</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-1153</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-1823</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-2311</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-2386</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2013-1635</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2014-8626</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2014-9427</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-5900</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-4889</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-3870</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-4697</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-4718</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-0831</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-5898</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-3659</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-2626</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1128</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1861</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-2191</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-0057</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-1172</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-4107</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2006-7243</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-4783</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-4840</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-4850</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-2666</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-3660</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-5498</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-1271</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-1272</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-3294</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-4418</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1130</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1860</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1862</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1864</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1914</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1915</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-1917</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-2093</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-2097</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-2100</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-2101</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-2190</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-2484</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-3065</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-4150</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-4645</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-4698</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-4699</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-0752</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-0755</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-1466</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-1467</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-2483</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-3182</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-3267</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-4885</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-0788</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-0789</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-1171</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-2336</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-3365</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2013-1643</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2013-2110</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2013-4635</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2014-0237</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2014-0238</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-4887</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-5447</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-5899</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2009-4142</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-2531</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-3709</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2010-3710</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-0421</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-0708</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-1464</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-1468</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-1469</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2011-1470</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2012-2143</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2013-4248</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2014-2497</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2014-5459</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2008-5814</p><p>http://www.cvedetails.com/cve-details.php?cve_id=CVE-2007-6039</p><p></p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">829</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">42</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-high">
<th width="20%"><a name="high"></a>High (Medium)</th><th width="80%">Source Code Disclosure - CVE-2012-1823</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Some PHP versions, when configured to run using CGI, do not correctly handle query strings that lack an unescaped "=" character, enabling PHP source code disclosure, and arbitrary code execution. In this case, the contents of the PHP file were served directly to the web browser. This output will typically contain PHP, although it may also contain straight HTML.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php?-s</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Upgrade to the latest stable version of PHP, or use the Apache web server and the mod_rewrite module to filter out malicious requests using the "RewriteCond" and "RewriteRule" directives.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>&lt;?php</p><p></p><p>// Lists the options from the array 'bugs' (bugs.txt)</p><p>foreach ($bugs as $key =&gt; $value)</p><p>{</p><p></p><p>   $bug = explode(",", trim($value));</p><p></p><p>   // Debugging</p><p>   // echo "key: " . $key;</p><p>   // echo " value: " . $bug[0];</p><p>   // echo " filename: " . $bug[1] . "&lt;br /&gt;";</p><p></p><p>   echo "&lt;option value='$key'&gt;$bug[0]&lt;/option&gt;";</p><p></p><p>}</p><p></p><p>?&gt;</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://projects.webappsec.org/Improper-Input-Handling</p><p>http://cwe.mitre.org/data/definitions/89.html</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">20</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">20</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-high">
<th width="20%"><a name="high"></a>High (Medium)</th><th width="80%">Remote Code Execution - CVE-2012-1823</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Some PHP versions, when configured to run using CGI, do not correctly handle query strings that lack an unescaped "=" character, enabling arbitrary code execution. In this case, an operating system command was caused to be executed on the web server, and the results were returned to the web browser. </p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php?-d+allow_url_include%3d1+-d+auto_prepend_file%3dphp://input</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">POST</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">&lt;?php exec('echo o0qml0i6tqk4mnhrtphh',$colm);echo join("
",$colm);die();?&gt;</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">o0qml0i6tqk4mnhrtphh</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Upgrade to the latest stable version of PHP, or use the Apache web server and the mod_rewrite module to filter out malicious requests using the "RewriteCond" and "RewriteRule" directives.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>o0qml0i6tqk4mnhrtphh</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://projects.webappsec.org/Improper-Input-Handling</p><p>http://cwe.mitre.org/data/definitions/89.html</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">20</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">20</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-medium">
<th width="20%"><a name="medium"></a>Medium (Medium)</th><th width="80%">HTTP Only Site</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The site is only served under HTTP and not HTTPS.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Configure your web or application server to use SSL (https).</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>Failed to connect.</p><p>ZAP attempted to connect via: https://192.168.150.10:443/bwapp/bWAPP</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://www.owasp.org/index.php/Transport_Layer_Protection_Cheat_Sheet</p><p>https://www.owasp.org/index.php/SSL_Best_Practices</p><p>https://letsencrypt.org/</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">311</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">4</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-medium">
<th width="20%"><a name="medium"></a>Medium (Medium)</th><th width="80%">Insecure HTTP Method - TRACE</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The insecure HTTP method [TRACE] is enabled for this resource, and is exploitable. The TRACK and TRACE methods may be used by an attacker, to gain access to the authorisation token/session cookie of an application user, even if the session cookie is protected using the 'HttpOnly' flag. For the attack to be successful, the application user must typically be using an older web browser, or a web browser which has a Same Origin Policy (SOP) bypass vulnerability.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">CnjIGY8BcdFYdYAfRw3FqXDMRBoLJCBcZe2sDOnx</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/twitter.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">6rlthkPHryQENIHEK84QWWdkjmenhvd96S2vUzkg</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/stylesheet.css</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">URw5frcK2jxpMoTRYBKhB4Rms3YRa2nk6wrVi7PQ</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bg_2.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">EgVqX8sPzzCgagK78G3z1TI9ECiluPrIr20OIay1</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/netsparker.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">hOztyiVDU2QZuynmeltPc4ZvVNiLNwand1hQ5sxR</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/linkedin.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">j2t8oumNWzn5nNx0BYOrjuNx0dITLErJcwfQQvUl</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/cc.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">Pjn4IH8sNXOBeDqS734QhwtvUx5R9rqZNxesqxmo</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/facebook.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">Jztle29D6GyqapMgaHJ1RMhvNnKthpfKSAjkLoyG</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/sb_1.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">zyx8k1yOl2OOX7tYuhtAnAxv9CUTq4dPFulkNVLB</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/html5.js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">EC813d2I8ZPdDroapGVcTOfrwCItKY8HarbVp0MV</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bg_3.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">sRb9GABLn9ooAWYktmL0xWSlGhPG28i1EJ4IZmNc</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/mk.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">PZ0JRflRD107zcaFCaPXfBmo3KNSow7GPmQ0POpx</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/owasp.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">oRi3Vzjhj0XTJXS1jhNnMLpc6VbVgyl5FblfcsbA</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bee_1.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">b291dVesucSe4hcHsOEeCnfXtR3lWS7joOjTJP3U</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bg_1.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">BhVrVIL1UaTErYx5mW7JmRbBkEC5Ziy8gjrJ0fes</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/zap.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">oU3eTYukl8PuCGdwPTxFJl7OYyDtLRXvgr29SPP9</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/blogger.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">TRACE</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">TzEm53oU1dVUJVnnpYFYn0y54RvHecbWkkHFif9R</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">17</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Disable insecure methods such as TRACK, TRACE, and CONNECT on the web server, and ensure that the underlying service implementation does not support insecure methods.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>A TRACE request was sent for this request, with a custom cookie value [CnjIGY8BcdFYdYAfRw3FqXDMRBoLJCBcZe2sDOnx]. This cookie value was disclosed in the HTTP response, confirming the vulnerability.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://projects.webappsec.org/Fingerprinting</p><p></p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">45</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-medium">
<th width="20%"><a name="medium"></a>Medium (Medium)</th><th width="80%">Apache Range Header DoS (CVE-2011-3192)</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The byterange filter in earlier versions of the Apache HTTP Server allows remote attackers to cause a denial of service (memory and CPU exhaustion) via a Range request header that identifies multiple overlapping ranges. This issue was exploited in the wild in August 2011.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/sb_1.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/mk.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/linkedin.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/owasp.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/blogger.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bee_1.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/cc.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/zap.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bg_3.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bg_1.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/netsparker.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bg_2.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/html5.js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/facebook.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/twitter.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/stylesheet.css</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 206 Partial Content</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">17</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Upgrade your Apache server to a currently stable version. Alternative solutions or workarounds are outlined in the references. </p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://httpd.apache.org/security/CVE-2011-3192.txt</p><p>http://cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3192</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">400</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">10</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-medium">
<th width="20%"><a name="medium"></a>Medium (Medium)</th><th width="80%">Relative Path Confusion</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The web server is configured to serve responses to ambiguous URLs in a manner that is likely to lead to confusion about the correct "relative path" for the URL. Resources (CSS, images, etc) are also specified in the page response using relative, rather than absolute URLs. In an attack, if the web browser parses the "cross-content" response in a permissive manner, or can be tricked into permissively parsing the "cross-content" response, using techniques such as framing, then the web browser may be fooled into interpreting HTML as CSS (or other content types), leading to an XSS vulnerability.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php/apei7/l330i</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">&lt;link rel="stylesheet" type="text/css" href="stylesheets/stylesheet.css" media="screen" /&gt;</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Web servers and frameworks should be updated to be configured to not serve responses to ambiguous URLs in such a way that the relative path of such URLs could be mis-interpreted by components on either the client side, or server side.</p><p>Within the application, the correct use of the "&lt;base&gt;" HTML tag in the HTTP response will unambiguously specify the base URL for all relative URLs in the document.</p><p>Use the "Content-Type" HTTP response header to make it harder for the attacker to force the web browser to mis-interpret the content type of the response.</p><p>Use the "X-Content-Type-Options: nosniff" HTTP response header to prevent the web browser from "sniffing" the content type of the response.</p><p>Use a modern DOCTYPE such as "&lt;!doctype html&gt;" to prevent the page from being rendered in the web browser using "Quirks Mode", since this results in the content type being ignored by the web browser.</p><p>Specify the "X-Frame-Options" HTTP response header to prevent Quirks Mode from being enabled in the web browser using framing attacks. </p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>No &lt;base&gt; tag was specified in the HTML &lt;head&gt; tag to define the location for relative URLs.</p><p>A Content Type of "text/html" was specified. If the web browser is employing strict parsing rules, this will prevent cross-content attacks from succeeding. Quirks Mode in the web browser would disable strict parsing.  </p><p>No X-Frame-Options header was specified, so the page can be framed, and this can be used to enable Quirks Mode, allowing the specified Content Type to be bypassed.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://www.thespanner.co.uk/2014/03/21/rpo/</p><p>https://hsivonen.fi/doctype/</p><p>http://www.w3schools.com/tags/tag_base.asp</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">20</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">20</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-medium">
<th width="20%"><a name="medium"></a>Medium (Medium)</th><th width="80%">X-Frame-Options Header Not Set</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>X-Frame-Options header is not included in the HTTP response to protect against 'ClickJacking' attacks.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">X-Frame-Options</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Most modern Web browsers support the X-Frame-Options HTTP header. Ensure it's set on all web pages returned by your site (if you expect the page to be framed only by pages on your server (e.g. it's part of a FRAMESET) then you'll want to use SAMEORIGIN, otherwise if you never expect the page to be framed, you should use DENY. ALLOW-FROM allows specific websites to frame the web page in supported web browsers).</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://blogs.msdn.com/b/ieinternals/archive/2010/03/30/combating-clickjacking-with-x-frame-options.aspx</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">16</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">15</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-medium">
<th width="20%"><a name="medium"></a>Medium (Medium)</th><th width="80%">Directory Browsing</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>It is possible to view the directory listing.  Directory listing may reveal hidden scripts, include files , backup source files etc which can be accessed to read sensitive information.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Parent Directory</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Parent Directory</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Parent Directory</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Parent Directory</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">4</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Disable directory browsing.  If this is required, make sure the listed files does not induce risks.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://httpd.apache.org/docs/mod/core.html#options</p><p>http://alamo.satlug.org/pipermail/satlug/2002-February/000053.html</p><p></p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">548</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">48</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-medium">
<th width="20%"><a name="medium"></a>Medium (Medium)</th><th width="80%">Reverse tabnabbing</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>At least one link on this page is vulnerable to Reverse tabnabbing as it uses a target attribute without using both of the "noopener" and "noreferrer" keywords in the "rel" attribute, which allows the target page to take control of this page.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">&lt;a href="http://itsecgames.blogspot.com" target="_blank"&gt;Blog&lt;/a&gt;</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Do not use a target attribute, or if you have to then also add the attribute: rel="noopener noreferrer".</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://www.owasp.org/index.php/Reverse_Tabnabbing</p><p>https://dev.to/ben/the-targetblank-vulnerability-by-example</p><p>https://mathiasbynens.github.io/rel-noopener/</p><p>https://medium.com/@jitbit/target-blank-the-most-underestimated-vulnerability-ever-96e328301f4c</p><p></p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-low">
<a name="low"></a><th width="20%">Low (High)</th><th width="80%">Server Leaks Version Information via "Server" HTTP Response Header Field</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The web/application server is leaking version information via the "Server" HTTP response header. Access to such information may facilitate attackers identifying other vulnerabilities your web/application server is subject to.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://detectportal.firefox.com/success.txt</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">AmazonS3</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Ensure that your web server, application server, load balancer, etc. is configured to suppress the "Server" header or provide generic details.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://httpd.apache.org/docs/current/mod/core.html#servertokens</p><p>http://msdn.microsoft.com/en-us/library/ff648552.aspx#ht_urlscan_007</p><p>http://blogs.msdn.com/b/varunm/archive/2013/04/23/remove-unwanted-http-response-headers.aspx</p><p>http://www.troyhunt.com/2012/02/shhh-dont-let-your-response-headers.html</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-low">
<a name="low"></a><th width="20%">Low (High)</th><th width="80%">Server Leaks Version Information via "Server" HTTP Response Header Field</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The web/application server is leaking version information via the "Server" HTTP response header. Access to such information may facilitate attackers identifying other vulnerabilities your web/application server is subject to.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">Apache/2.2.8 (Ubuntu) DAV/2</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/html5.js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">Apache/2.2.8 (Ubuntu) DAV/2</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">Apache/2.2.8 (Ubuntu) DAV/2</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/stylesheet.css</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">Apache/2.2.8 (Ubuntu) DAV/2</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">4</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Ensure that your web server, application server, load balancer, etc. is configured to suppress the "Server" header or provide generic details.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://httpd.apache.org/docs/current/mod/core.html#servertokens</p><p>http://msdn.microsoft.com/en-us/library/ff648552.aspx#ht_urlscan_007</p><p>http://blogs.msdn.com/b/varunm/archive/2013/04/23/remove-unwanted-http-response-headers.aspx</p><p>http://www.troyhunt.com/2012/02/shhh-dont-let-your-response-headers.html</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-low">
<a name="low"></a><th width="20%">Low (Medium)</th><th width="80%">X-Content-Type-Options Header Missing</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The Anti-MIME-Sniffing header X-Content-Type-Options was not set to 'nosniff'. This allows older versions of Internet Explorer and Chrome to perform MIME-sniffing on the response body, potentially causing the response body to be interpreted and displayed as a content type other than the declared content type. Current (early 2014) and legacy versions of Firefox will use the declared content type (if one is set), rather than performing MIME-sniffing.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://detectportal.firefox.com/success.txt</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">X-Content-Type-Options</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Ensure that the application/web server sets the Content-Type header appropriately, and that it sets the X-Content-Type-Options header to 'nosniff' for all web pages.</p><p>If possible, ensure that the end user uses a standards-compliant and modern web browser that does not perform MIME-sniffing at all, or that can be directed by the web application/web server to not perform MIME-sniffing.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>This issue still applies to error type pages (401, 403, 500, etc) as those pages are often still affected by injection issues, in which case there is still concern for browsers sniffing pages away from their actual content type.</p><p>At "High" threshold this scanner will not alert on client or server error responses.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://msdn.microsoft.com/en-us/library/ie/gg622941%28v=vs.85%29.aspx</p><p>https://www.owasp.org/index.php/List_of_useful_HTTP_headers</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">16</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">15</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-low">
<a name="low"></a><th width="20%">Low (Medium)</th><th width="80%">Web Browser XSS Protection Not Enabled</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Web Browser XSS Protection is not enabled, or is disabled by the configuration of the 'X-XSS-Protection' HTTP response header on the web server</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">X-XSS-Protection</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Ensure that the web browser's XSS filter is enabled, by setting the X-XSS-Protection HTTP response header to '1'.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>The X-XSS-Protection HTTP response header allows the web server to enable or disable the web browser's XSS protection mechanism. The following values would attempt to enable it: </p><p>X-XSS-Protection: 1; mode=block</p><p>X-XSS-Protection: 1; report=http://www.example.com/xss</p><p>The following values would disable it:</p><p>X-XSS-Protection: 0</p><p>The X-XSS-Protection HTTP response header is currently supported on Internet Explorer, Chrome and Safari (WebKit).</p><p>Note that this alert is only raised if the response body could potentially contain an XSS payload (with a text-based content type, with a non-zero length).</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet</p><p>https://blog.veracode.com/2014/03/guidelines-for-setting-security-headers/</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">933</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">14</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-low">
<a name="low"></a><th width="20%">Low (Medium)</th><th width="80%">X-Content-Type-Options Header Missing</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The Anti-MIME-Sniffing header X-Content-Type-Options was not set to 'nosniff'. This allows older versions of Internet Explorer and Chrome to perform MIME-sniffing on the response body, potentially causing the response body to be interpreted and displayed as a content type other than the declared content type. Current (early 2014) and legacy versions of Firefox will use the declared content type (if one is set), rather than performing MIME-sniffing.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/html5.js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">X-Content-Type-Options</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/stylesheet.css</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">X-Content-Type-Options</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">X-Content-Type-Options</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">X-Content-Type-Options</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">4</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Ensure that the application/web server sets the Content-Type header appropriately, and that it sets the X-Content-Type-Options header to 'nosniff' for all web pages.</p><p>If possible, ensure that the end user uses a standards-compliant and modern web browser that does not perform MIME-sniffing at all, or that can be directed by the web application/web server to not perform MIME-sniffing.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>This issue still applies to error type pages (401, 403, 500, etc) as those pages are often still affected by injection issues, in which case there is still concern for browsers sniffing pages away from their actual content type.</p><p>At "High" threshold this scanner will not alert on client or server error responses.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://msdn.microsoft.com/en-us/library/ie/gg622941%28v=vs.85%29.aspx</p><p>https://www.owasp.org/index.php/List_of_useful_HTTP_headers</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">16</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">15</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-low">
<a name="low"></a><th width="20%">Low (Medium)</th><th width="80%">Отсутствуют токены против CSRF атак</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Токены для обезвреживания атак CSRF не были обнаружены в форме отправки на странице HTML.</p><p>A cross-site request forgery is an attack that involves forcing a victim to send an HTTP request to a target destination without their knowledge or intent in order to perform an action as the victim. The underlying cause is application functionality using predictable URL/form actions in a repeatable way. The nature of the attack is that CSRF exploits the trust that a web site has for a user. By contrast, cross-site scripting (XSS) exploits the trust that a user has for a web site. Like XSS, CSRF attacks are not necessarily cross-site, but they can be. Cross-site request forgery is also known as CSRF, XSRF, one-click attack, session riding, confused deputy, and sea surf.</p><p></p><p>CSRF attacks are effective in a number of situations, including:</p><p>    * The victim has an active session on the target site.</p><p>    * The victim is authenticated via HTTP auth on the target site.</p><p>    * The victim is on the same local network as the target site.</p><p></p><p>CSRF has primarily been used to perform an action against a target site using the victim's privileges, but recent techniques have been discovered to disclose information by gaining access to the response. The risk of information disclosure is dramatically increased when the target site is vulnerable to XSS, because XSS can be used as a platform for CSRF, allowing the attack to operate within the bounds of the same-origin policy.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">&lt;form action="/bwapp/bWAPP/portal.php" method="POST"&gt;</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">&lt;form action="/bwapp/bWAPP/portal.php" method="POST"&gt;</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">&lt;form action="/bwapp/bWAPP/portal.php" method="POST"&gt;</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">3</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Phase: Architecture and Design</p><p>Use a vetted library or framework that does not allow this weakness to occur or provides constructs that make this weakness easier to avoid.</p><p>For example, use anti-CSRF packages such as the OWASP CSRFGuard.</p><p></p><p>Phase: Implementation</p><p>Ensure that your application is free of cross-site scripting issues, because most CSRF defenses can be bypassed using attacker-controlled script.</p><p></p><p>Phase: Architecture and Design</p><p>Generate a unique nonce for each form, place the nonce into the form, and verify the nonce upon receipt of the form. Be sure that the nonce is not predictable (CWE-330).</p><p>Note that this can be bypassed using XSS.</p><p></p><p>Identify especially dangerous operations. When the user performs a dangerous operation, send a separate confirmation request to ensure that the user intended to perform that operation.</p><p>Note that this can be bypassed using XSS.</p><p></p><p>Use the ESAPI Session Management control.</p><p>This control includes a component for CSRF.</p><p></p><p>Do not use the GET method for any request that triggers a state change.</p><p></p><p>Phase: Implementation</p><p>Check the HTTP Referer header to see if the request originated from an expected page. This could break legitimate functionality, because users or proxies may have disabled sending the Referer for privacy reasons.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>Токены против атак CSRF [anticsrf, CSRFToken, __RequestVerificationToken, csrfmiddlewaretoken, authenticity_token, OWASP_CSRFTOKEN, anoncsrf] не были обнаружены в следующих формах HTML: [Form 3: ].  </p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://projects.webappsec.org/Cross-Site-Request-Forgery</p><p>http://cwe.mitre.org/data/definitions/352.html</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">352</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">9</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-low">
<a name="low"></a><th width="20%">Low (Medium)</th><th width="80%">Server Leaks Information via "X-Powered-By" HTTP Response Header Field(s)</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The web/application server is leaking information via one or more "X-Powered-By" HTTP response headers. Access to such information may facilitate attackers identifying other frameworks/components your web application is reliant upon and the vulnerabilities such components may be subject to.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">X-Powered-By: PHP/5.2.4-2ubuntu5.10</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Ensure that your web server, application server, load balancer, etc. is configured to suppress "X-Powered-By" headers.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://blogs.msdn.com/b/varunm/archive/2013/04/23/remove-unwanted-http-response-headers.aspx</p><p>http://www.troyhunt.com/2012/02/shhh-dont-let-your-response-headers.html</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-low">
<a name="low"></a><th width="20%">Low (Medium)</th><th width="80%">Content Security Policy (CSP) Header Not Set</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Content Security Policy (CSP) is an added layer of security that helps to detect and mitigate certain types of attacks, including Cross Site Scripting (XSS) and data injection attacks. These attacks are used for everything from data theft to site defacement or distribution of malware. CSP provides a set of standard HTTP headers that allow website owners to declare approved sources of content that browsers should be allowed to load on that page &mdash; covered types are JavaScript, CSS, HTML frames, fonts, images and embeddable objects such as Java applets, ActiveX, audio and video files.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Ensure that your web server, application server, load balancer, etc. is configured to set the Content-Security-Policy header, to achieve optimal browser support: "Content-Security-Policy" for Chrome 25+, Firefox 23+ and Safari 7+, "X-Content-Security-Policy" for Firefox 4.0+ and Internet Explorer 10+, and "X-WebKit-CSP" for Chrome 14+ and Safari 6+.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://developer.mozilla.org/en-US/docs/Web/Security/CSP/Introducing_Content_Security_Policy</p><p>https://www.owasp.org/index.php/Content_Security_Policy</p><p>http://www.w3.org/TR/CSP/</p><p>http://w3c.github.io/webappsec/specs/content-security-policy/csp-specification.dev.html</p><p>http://www.html5rocks.com/en/tutorials/security/content-security-policy/</p><p>http://caniuse.com/#feat=contentsecuritypolicy</p><p>http://content-security-policy.com/</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">16</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">15</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-low">
<a name="low"></a><th width="20%">Low (Low)</th><th width="80%">Hash Disclosure - MD4 / MD5</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>A hash was disclosed by the web server - MD4 / MD5</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://detectportal.firefox.com/success.txt</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">ae780585f49b94ce1444eb7d28906123</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Ensure that hashes that are used to protect credentials or other resources are not leaked by the web server or database. There is typically no requirement for password hashes to be accessible to the web browser.      </p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>ae780585f49b94ce1444eb7d28906123</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://www.owasp.org/index.php/Top_10_2013-A6-Sensitive_Data_Exposure</p><p>http://projects.webappsec.org/w/page/13246936/Information%20Leakage</p><p>http://openwall.info/wiki/john/sample-hashes</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-low">
<a name="low"></a><th width="20%">Low (Low)</th><th width="80%">Hash Disclosure - MD4 / MD5</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>A hash was disclosed by the web server - MD4 / MD5</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">c7995a01a2cde2fee403b44fa0b90ec5</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/stylesheet.css</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">c7995a01a2cde2fee403b44fa0b90ec5</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">c7995a01a2cde2fee403b44fa0b90ec5</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/html5.js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">c7995a01a2cde2fee403b44fa0b90ec5</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">4</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Ensure that hashes that are used to protect credentials or other resources are not leaked by the web server or database. There is typically no requirement for password hashes to be accessible to the web browser.      </p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>c7995a01a2cde2fee403b44fa0b90ec5</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://www.owasp.org/index.php/Top_10_2013-A6-Sensitive_Data_Exposure</p><p>http://projects.webappsec.org/w/page/13246936/Information%20Leakage</p><p>http://openwall.info/wiki/john/sample-hashes</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-info">
<th width="20%"><a name="info"></a>Informational (High)</th><th width="80%">.htaccess Information Leak</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>htaccess files can be used to alter the configuration of the Apache Web Server software to enable/disable additional functionality and features that the Apache Web Server software has to offer. </p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/.htaccess</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 403 Forbidden</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/.htaccess</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 403 Forbidden</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/.htaccess</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 403 Forbidden</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/.htaccess</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 403 Forbidden</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/.htaccess</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 403 Forbidden</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/.htaccess</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">HTTP/1.1 403 Forbidden</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">6</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Ensure the .htaccess file is not accessible.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>Based on response status code htaccess file may be protected by an authentication or authorization mechanism.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://www.htaccess-guide.com/</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">215</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-info">
<th width="20%"><a name="info"></a>Informational (Medium)</th><th width="80%">Base64 Disclosure</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Base64 encoded data was disclosed by the application/web server</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://detectportal.firefox.com/success.txt</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">MnfbeXeS3ep60gjgpK6jEZF5WYcQix8AeNXFZBLf8RpVEOC1kWBUUQ==</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://detectportal.firefox.com/success.txt</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">XzFHsVNetMNLaMez4UH5lr3M6gYjPtoqfOt5jKMXSsV4pQw41BHvrw==</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">2</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Manually confirm that the Base64 data does not leak sensitive information, and that the data cannot be aggregated/used to exploit other vulnerabilities.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>2w�yw���z�\x0008म�\x0011�yY�\x0010�\x001f\x0000x��d\x0012��\x001aU\x0010൑`TQ</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://www.owasp.org/index.php/Top_10_2013-A6-Sensitive_Data_Exposure</p><p>http://projects.webappsec.org/w/page/13246936/Information%20Leakage</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-info">
<th width="20%"><a name="info"></a>Informational (Medium)</th><th width="80%">Non-Storable Content</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The response contents are not storable by caching components such as proxy servers. If the response does not contain sensitive, personal or user-specific information, it may benefit from being stored and cached, to improve performance.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://detectportal.firefox.com/success.txt</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">no-store</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>The content may be marked as storable by ensuring that the following conditions are satisfied:</p><p>The request method must be understood by the cache and defined as being cacheable ("GET", "HEAD", and "POST" are currently defined as cacheable)</p><p>The response status code must be understood by the cache (one of the 1XX, 2XX, 3XX, 4XX, or 5XX response classes are generally understood)</p><p>The "no-store" cache directive must not appear in the request or response header fields</p><p>For caching by "shared" caches such as "proxy" caches, the "private" response directive must not appear in the response</p><p>For caching by "shared" caches such as "proxy" caches, the "Authorization" header field must not appear in the request, unless the response explicitly allows it (using one of the "must-revalidate", "public", or "s-maxage" Cache-Control response directives)</p><p>In addition to the conditions above, at least one of the following conditions must also be satisfied by the response:</p><p>It must contain an "Expires" header field</p><p>It must contain a "max-age" response directive</p><p>For "shared" caches such as "proxy" caches, it must contain a "s-maxage" response directive</p><p>It must contain a "Cache Control Extension" that allows it to be cached</p><p>It must have a status code that is defined as cacheable by default (200, 203, 204, 206, 300, 301, 404, 405, 410, 414, 501).   </p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://tools.ietf.org/html/rfc7234</p><p>https://tools.ietf.org/html/rfc7231</p><p>http://www.w3.org/Protocols/rfc2616/rfc2616-sec13.html (obsoleted by rfc7234)</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">524</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-info">
<th width="20%"><a name="info"></a>Informational (Medium)</th><th width="80%">User Agent Fuzzer</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Check for differences in response based on fuzzed User Agent (eg. mobile sites, access as a Search Engine Crawler). Compares the response statuscode and the hashcode of the response body with the original response.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (iPhone; U; CPU iPhone OS 3_0 like Mac OS X; en-us) AppleWebKit/528.18 (KHTML, like Gecko) Version/4.0 Mobile/7A341 Safari/528.16</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (compatible; Yahoo! Slurp; http://help.yahoo.com/help/us/ysearch/slurp)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.0)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (compatible; Yahoo! Slurp; http://help.yahoo.com/help/us/ysearch/slurp)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.0)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (compatible; Yahoo! Slurp; http://help.yahoo.com/help/us/ysearch/slurp)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (iPhone; U; CPU iPhone OS 3_0 like Mac OS X; en-us) AppleWebKit/528.18 (KHTML, like Gecko) Version/4.0 Mobile/7A341 Safari/528.16</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">msnbot/1.1 (+http://search.msn.com/msnbot.htm)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (compatible; Yahoo! Slurp; http://help.yahoo.com/help/us/ysearch/slurp)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">msnbot/1.1 (+http://search.msn.com/msnbot.htm)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">msnbot/1.1 (+http://search.msn.com/msnbot.htm)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (iPhone; U; CPU iPhone OS 3_0 like Mac OS X; en-us) AppleWebKit/528.18 (KHTML, like Gecko) Version/4.0 Mobile/7A341 Safari/528.16</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Parameter</td><td width="80%">Header User-Agent</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Attack</td><td width="80%">Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.1)</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">35</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p></p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://www.owasp.org/index.php/Web_Application_Security_Testing_Cheat_Sheet</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-info">
<th width="20%"><a name="info"></a>Informational (Medium)</th><th width="80%">Storable and Cacheable Content</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The response contents are storable by caching components such as proxy servers, and may be retrieved directly from the cache, rather than from the origin server by the caching servers, in response to similar requests from other users.  If the response data is sensitive, personal or user-specific, this may result in sensitive information being leaked. In some cases, this may even result in a user gaining complete control of the session of another user, depending on the configuration of the caching components in use in their environment. This is primarily an issue where "shared" caching servers such as "proxy" caches are configured on the local network. This configuration is typically found in corporate or educational environments, for instance.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/stylesheet.css</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/html5.js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">3</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Validate that the response does not contain sensitive, personal or user-specific information.  If it does, consider the use of the following HTTP response headers, to limit, or prevent the content being stored and retrieved from the cache by another user:</p><p>Cache-Control: no-cache, no-store, must-revalidate, private</p><p>Pragma: no-cache</p><p>Expires: 0</p><p>This configuration directs both HTTP 1.0 and HTTP 1.1 compliant caching servers to not store the response, and to not retrieve the response (without validation) from the cache, in response to a similar request. </p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>In the absence of an explicitly specified caching lifetime directive in the response, a liberal lifetime heuristic of 1 year was assumed. This is permitted by rfc7234.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://tools.ietf.org/html/rfc7234</p><p>https://tools.ietf.org/html/rfc7231</p><p>http://www.w3.org/Protocols/rfc2616/rfc2616-sec13.html (obsoleted by rfc7234)</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">524</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-info">
<th width="20%"><a name="info"></a>Informational (Medium)</th><th width="80%">Base64 Disclosure</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Base64 encoded data was disclosed by the application/web server</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">com/pages/MME-IT-Audits-Security/104153019664877</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Manually confirm that the Base64 data does not leak sensitive information, and that the data cannot be aggregated/used to exploit other vulnerabilities.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>r����\x001e��\x000c\x0013�\x0013�\x000b���&gt;I�.�+r�]8ם��޺���</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://www.owasp.org/index.php/Top_10_2013-A6-Sensitive_Data_Exposure</p><p>http://projects.webappsec.org/w/page/13246936/Information%20Leakage</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-info">
<th width="20%"><a name="info"></a>Informational (Medium)</th><th width="80%">Information Disclosure - Suspicious Comments</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The response appears to contain suspicious comments which may help an attacker.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/html5.js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Remove all comments that return information that may help an attacker and fix any underlying problems they refer to.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>(function(a,b){function h(a,b){var c=a.createElement("p"),d=a.getElementsByTagName("head")[0]||a.documentElement;return c.innerHTML="x&lt;style&gt;"+b+"&lt;/style&gt;",d.insertBefore(c.lastChild,d.firstChild)}function i(){var a=l.elements;return typeof a=="string"?a.split(" "):a}function j(a){var b={},c=a.createElement,f=a.createDocumentFragment,g=f();a.createElement=function(a){if(!l.shivMethods)return c(a);var f;return b[a]?f=b[a].cloneNode():e.test(a)?f=(b[a]=c(a)).cloneNode():f=c(a),f.canHaveChildren&amp;&amp;!d.test(a)?g.appendChild(f):f},a.createDocumentFragment=Function("h,f","return function(){var n=f.cloneNode(),c=n.createElement;h.shivMethods&amp;&amp;("+i().join().replace(/\w+/g,function(a){return c(a),g.createElement(a),'c("'+a+'")'})+");return n}")(l,g)}function k(a){var b;return a.documentShived?a:(l.shivCSS&amp;&amp;!f&amp;&amp;(b=!!h(a,"article,aside,details,figcaption,figure,footer,header,hgroup,nav,section{display:block}audio{display:none}canvas,video{display:inline-block;*display:inline;*zoom:1}[hidden]{display:none}audio[controls]{display:inline-block;*display:inline;*zoom:1}mark{background:#FF0;color:#000}")),g||(b=!j(a)),b&amp;&amp;(a.documentShived=b),a)}var c=a.html5||{},d=/^&lt;|^(?:button|form|map|select|textarea|object|iframe|option|optgroup)$/i,e=/^&lt;|^(?:a|b|button|code|div|fieldset|form|h1|h2|h3|h4|h5|h6|i|iframe|img|input|label|li|link|ol|option|p|param|q|script|select|span|strong|style|table|tbody|td|textarea|tfoot|th|thead|tr|ul)$/i,f,g;(function(){var c=b.createElement("a");c.innerHTML="&lt;xyz&gt;&lt;/xyz&gt;",f="hidden"in c,f&amp;&amp;typeof injectElementWithStyles=="function"&amp;&amp;injectElementWithStyles("#modernizr{}",function(b){b.hidden=!0,f=(a.getComputedStyle?getComputedStyle(b,null):b.currentStyle).display=="none"}),g=c.childNodes.length==1||function(){try{b.createElement("a")}catch(a){return!0}var c=b.createDocumentFragment();return typeof c.cloneNode=="undefined"||typeof c.createDocumentFragment=="undefined"||typeof c.createElement=="undefined"}()})();var l={elements:c.elements||"abbr article aside audio bdi canvas data datalist details figcaption figure footer header hgroup mark meter nav output progress section summary time video",shivCSS:c.shivCSS!==!1,shivMethods:c.shivMethods!==!1,type:"default",shivDocument:k};a.html5=l,k(b)})(this,document)</p><p></p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p></p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-info">
<th width="20%"><a name="info"></a>Informational (Medium)</th><th width="80%">Non-Storable Content</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>The response contents are not storable by caching components such as proxy servers. If the response does not contain sensitive, personal or user-specific information, it may benefit from being stored and cached, to improve performance.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/portal.php</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">no-store</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">1</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>The content may be marked as storable by ensuring that the following conditions are satisfied:</p><p>The request method must be understood by the cache and defined as being cacheable ("GET", "HEAD", and "POST" are currently defined as cacheable)</p><p>The response status code must be understood by the cache (one of the 1XX, 2XX, 3XX, 4XX, or 5XX response classes are generally understood)</p><p>The "no-store" cache directive must not appear in the request or response header fields</p><p>For caching by "shared" caches such as "proxy" caches, the "private" response directive must not appear in the response</p><p>For caching by "shared" caches such as "proxy" caches, the "Authorization" header field must not appear in the request, unless the response explicitly allows it (using one of the "must-revalidate", "public", or "s-maxage" Cache-Control response directives)</p><p>In addition to the conditions above, at least one of the following conditions must also be satisfied by the response:</p><p>It must contain an "Expires" header field</p><p>It must contain a "max-age" response directive</p><p>For "shared" caches such as "proxy" caches, it must contain a "s-maxage" response directive</p><p>It must contain a "Cache Control Extension" that allows it to be cached</p><p>It must have a status code that is defined as cacheable by default (200, 203, 204, 206, 300, 301, 404, 405, 410, 414, 501).   </p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://tools.ietf.org/html/rfc7234</p><p>https://tools.ietf.org/html/rfc7231</p><p>http://www.w3.org/Protocols/rfc2616/rfc2616-sec13.html (obsoleted by rfc7234)</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">524</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-info">
<th width="20%"><a name="info"></a>Informational (Low)</th><th width="80%">Timestamp Disclosure - Unix</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>A timestamp was disclosed by the application/web server - Unix</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">74767232</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">546367672</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">327276754</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">76354632</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">476763262</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/stylesheet.css</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">20110126</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">76767632</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">54767654</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Evidence</td><td width="80%">546367547</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">9</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p>Manually confirm that the timestamp data is not sensitive, and that the data cannot be aggregated to disclose exploitable patterns.</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>74767232, which evaluates to: 1972-05-15 15:40:32</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>https://www.owasp.org/index.php/Top_10_2013-A6-Sensitive_Data_Exposure</p><p>http://projects.webappsec.org/w/page/13246936/Information%20Leakage</p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">13</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">3</td>
</tr>

</table>
<div class="spacer"></div>
<table width="100%" class="results">
  
  
  
<tr height="24" class="risk-info">
<th width="20%"><a name="info"></a>Informational (Low)</th><th width="80%">Сканер уязвимостей Cookie</th>
</tr>
  
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Description</td><td width="80%"><p>Repeated GET requests: drop a different cookie each time, followed by normal request with all cookies to stabilize session, compare responses against original baseline GET. This can reveal areas where cookie based authentication/attributes are not actually enforced.</p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/twitter.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/mk.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/linkedin.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts/architectsdaughter.ttf</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bg_3.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/cc.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bg_2.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/facebook.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/netsparker.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/js/html5.js</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/zap.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/owasp.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bg_1.jpg</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/stylesheets/stylesheet.css</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/fonts</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent1">URL</td><td width="80%">http://192.168.150.10/bwapp/bWAPP/images/bee_1.png</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%" class="indent2">Method</td><td width="80%">GET</td>
</tr>
  
  
  
<tr bgcolor="#e8e8e8">
<td width="20%">Instances</td><td width="80%">22</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Solution</td><td width="80%"><p></p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Other information</td><td width="80%"><p>Cookies that don't have expected effects can reveal flaws in application logic. In the worst case, this can reveal where authentication via cookie token(s) is not actually enforced.</p><p>Эти cookies изменили ответ: </p><p>Эти cookies не поменяли ответ: PHPSESSID,security_level</p><p></p></td>
</tr>
<TR vAlign="top">
<TD colspan="2"></TD>
</TR>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Reference</td><td width="80%"><p>http://projects.webappsec.org/Fingerprinting</p><p></p></td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">CWE Id</td><td width="80%">200</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">WASC Id</td><td width="80%">45</td>
</tr>
  
<tr bgcolor="#e8e8e8">
<td width="20%">Source ID</td><td width="80%">1</td>
</tr>


</table>
</body>
</html>
