---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


graphClient.Security().Cases().EdiscoveryCasesById("ediscoveryCase-id").ReviewSetsById("ediscoveryReviewSet-id").QueriesById("ediscoveryReviewSetQuery-id").Delete(context.Background(), nil)


```