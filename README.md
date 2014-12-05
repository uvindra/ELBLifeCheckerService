ELBLifeCheckerService
=====================

This is a custom Axis2 service for checking the availablility of the WSO2 ELB.

The service is packaged as a OSGi bundle.

Due to the "$" characters used in the name of this service you need to invoke it with escape characters as follows,
	
	curl -v -H "Content-Type: text/xml; charset=utf-8" -H "SOAPAction:" -X GET http://localhost:8280/services/ELB_LIFE_CHECKER_\$\$_SERVICE/pingService

The "$" characters were used to make the name uncommon  so that it would not clash with an existing/commonly used service name 
