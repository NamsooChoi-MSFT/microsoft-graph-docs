---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
	"@odata.id": "https://graph.microsoft.com/v1.0/groups/{id}",
}
options := &msgraphsdk.DirectoryObjectRequestBuilderPostOptions{
	Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
directoryObjectId := "directoryObject-id"
graphClient.Directory().AdministrativeUnitsById(&administrativeUnitId).MembersById(&directoryObjectId).Post(options)


```