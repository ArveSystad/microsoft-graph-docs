---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewSetVerifiedPublisherPostRequestBody()
verifiedPublisherId := "1234567"
requestBody.SetVerifiedPublisherId(&verifiedPublisherId) 

graphClient.ApplicationsById("application-id").SetVerifiedPublisher().Post(context.Background(), requestBody, nil)


```