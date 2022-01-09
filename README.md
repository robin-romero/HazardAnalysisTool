# HazardAnalysisTool
The Hazard Analysis Tool is used to determine the severity of a harm that may occur due to a sequence of foreseeable events. Each harm has a set of mitigators in place to reduce the severity of the harm with verifiers in place to validate/verify each mitigator. Each FSOE(Foreseeable Sequence of Events) is linked to one another to display what events may take place that lead to a single or set of hazards that in turn lead to a harm.

<img width="1680" alt="FullDiagramView" src="https://user-images.githubusercontent.com/43802156/148664991-132aa846-3609-4d0f-bb26-bedb05bac7ee.png">
This is the full HAT diagram view. Each node is shown connected to another node or set of nodes which determines the sequence of events from one node to another. Towards the end of the sequence of events the final event node leads to a hazard node that is then connected to the final harm. The harm dictates what events may take place that lead to this certain harm.

<img width="1680" alt="DiagramViewFullDepthFromSource" src="https://user-images.githubusercontent.com/43802156/148664990-97d08a9c-7885-477e-a7b5-b19ae80031c1.png">
With a node or set of nodes selected the user may then check what the events may take place from the selected node. The user is also able to control the depth that displays the sequence of events. In this case the depth leads all the way to the harms.

<img width="1680" alt="DiagramDepthLeft3" src="https://user-images.githubusercontent.com/43802156/148664998-ef786e17-08e0-4d59-ac5b-fed3232166de.png">
This diagram shows that the user has set the depth to be up to 3 nodes deep towards the root source of the selected node(s).

<img width="1680" alt="DiagramDepthRight3" src="https://user-images.githubusercontent.com/43802156/148664999-69480d0a-bd5b-407d-a4ca-da807becaa42.png">
This diagram shows that the user set the depth of nodes to be up to 3 nodes deep towards the harm of the selected node(s).

<img width="1680" alt="DataView" src="https://user-images.githubusercontent.com/43802156/148665003-118055b8-90ed-4f42-9f89-63371326d416.png">
This is the HAT data view. This displays all the previously shown nodes in a table row format. Each node displays the name of the node along with its ID.

<img width="1680" alt="EditSource" src="https://user-images.githubusercontent.com/43802156/148665000-faa9a0b8-8e48-4657-ab0b-a968c719eb9e.png">
Each row is able to be edited within the app. When editing a node all changes are updated in the realm database and is then updated in the table.

<img width="1501" alt="CreateNewNode" src="https://user-images.githubusercontent.com/43802156/148665005-aff8c7f5-c529-46a2-88dd-0f8f281776a1.png">
The user is able to create a new node be it a source, event, harm or link. A source is the root node for the sequence of events, an event is a single event that takes place in the sequence, a hazard is a possible lead to a harm, a harm is the outcome of the sequence of events, a mitigator is used to reduce a harm's severity, a verifier is used to validate the mitigators, and finally a link is the data that links the sequence between two nodes.

<img width="1680" alt="ImportSetting" src="https://user-images.githubusercontent.com/43802156/148664993-0731be51-6233-47e7-86ec-c259860d8567.png">
The user is able to import data to update the database of the application in turn updating the data view and diagram view as long as the data is in Json format.

<img width="1680" alt="SeveritySetting" src="https://user-images.githubusercontent.com/43802156/148664996-75ee8b09-8222-46fa-ac87-59ba2a4c0d0d.png">
This setting is used to change the description for each level of severity that is possible in the application.

<img width="1680" alt="MitigatorOccurrenceSetting" src="https://user-images.githubusercontent.com/43802156/148664997-118f1c3a-b74b-462c-a90b-5e7ce1b689a3.png">
This setting is used to change the description of each occurrence frequency of a link that exists between two nodes.


The following will display the data in Json format. The application exports its data in Json format and accepts imported data in Json format.
<img width="1680" alt="SourceJson" src="https://user-images.githubusercontent.com/43802156/148665006-7a244b47-12fe-4710-8262-b5eebeabb2aa.png">
This is the source nodes in Json format. 

<img width="1680" alt="LinkJson" src="https://user-images.githubusercontent.com/43802156/148665002-2bfc46cc-24c4-47b1-9f05-f882be7e28df.png">
This is the links in Json format with their set of mitigators.

<img width="1680" alt="MitigatorJson" src="https://user-images.githubusercontent.com/43802156/148665004-254aafe7-b527-4938-af8f-4212f5a85f8c.png">
This is the mitigators with their set of verifiers in Json format.
