# SOSL_GetFlowList
This is for get list of flow from the org 
(https://developer.salesforce.com/forums/?id=9062I000000QvDzQAK) 

SELECT ApiName, TriggerType, Label FROM FlowDefinitionView WHERE IsActive =true 

you can easily query it through SOQL.
1. Go to you developer console 
2. Select 'Query Editor'
3. In query editor check this option 'Use Tooling API'
4. Run the following query
Select id,MasterLabel,lastmodifieddate,lastmodifiedby.name from flow Where MasterLabel = 'Opportunity Status Change'
