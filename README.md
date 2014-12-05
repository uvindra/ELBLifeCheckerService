ELBLifeCheckerService
=====================

This is a custom Axis2 service for checking the availablility of the WSO2 ELB.

The service is packaged as a OSGi bundle.

Installation
------------
Since this is packaged as an OSGi bundle, copy the ELBLifeCheckerService_1.0.0.jar file to \<CARBON_SERVER\>/repository/components/dropins to install


Service Invocation
------------------
Due to the "$" characters used in the name of this service you need to invoke it with escape characters as follows,
	
	curl -v -H "Content-Type: text/xml; charset=utf-8" -H "SOAPAction:" -X GET http://localhost:8280/services/ELB_LIFE_CHECKER_\$\$_SERVICE/pingService

The "$" characters were used to make the name uncommon  so that it would not clash with an existing/commonly used service name 
