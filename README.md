# reziPHP
Rezi PHP Class for quick integration for web devs


Hello, This is a simple php class designed to be included in composer based projects. It should allow web developers to quickly implement rezi property search functionality within their website projects.

<h2>Usage</h2>

Initiate the class via:

<pre>$rezi = new Rezi($apikey, $clientsecret, $clientID, $environment);</pre>

Authentication is already done for you on class __construct

NOTE: The $apikey variable should be set to <strong>false</strong> if you are using a client secret and ID. The class will save the returned access token to a randomly named txt file.

Call an endpoint by:

<pre>$rezi->getRezi($type, $endpoint, $pagesize = false, $pagenumber = false, $payload = false, $qstring = false)</pre>

The JSON encoded results are automatically decoded into a PHP array ready for use.

WARNING: Ensure directory indexing is OFF in apache or nginx, otherwise someone could find your access token.

<h3>New Features will be added as they become available in Rezi.</h3>

Have Fun!
