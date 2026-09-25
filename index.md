<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
window.addEventListener("onEmbeddedMessagingReady", function() {
	console.log("Received the onEmbeddedMessagingReady event…");
            embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({
                "Card_Token": "12345"
            });
        });
			embeddedservice_bootstrap.init(
				'00DRT00000AsqQT',
				'Amazon_Messaging',
				'https://fleetcorna--uat.sandbox.my.site.com/ESWAmazonMessaging1761138530537',
				{
					scrt2URL: 'https://fleetcorna--uat.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://fleetcorna--uat.sandbox.my.site.com/ESWAmazonMessaging1761138530537/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
