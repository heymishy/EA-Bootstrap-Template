TODO


##PHASE 1 PLAN

re-jig the standard EA html output template to build own template from static content.

use the .xml generated into ~/js/data/*.xml 

e.g. 
	tocTab[tocTab.length] = new Array("0.7.2:1", "", "Credit Suisse Requirements", "EARoot/EA7/EA2/EA1085.html", "188.png", "2764", "0", "", "Custom diagram0","{1FEE8BE4-B9E8-48de-98C9-DE110A3A6F14}");

Filename = Package GUID

PackageHeirarchy, *?* , Element Name, relative path to content, nav icon, *? diagram ID? * , *?* ,  *?* , Diagram Type,

##PHASE 2 PLAN

example SQL for looking at single diagram (use case with relevant elements including links)

	select * from t_diagram where Name = '100 - Trading Use Cases'
	select * from t_object where Package_ID = '3424'
	select * from t_diagramobjects where Diagram_ID = '3182'
	select * from t_diagramlinks where DiagramID = '3182'

Possible JS diagram library

* jsPlumb
* arborjs



