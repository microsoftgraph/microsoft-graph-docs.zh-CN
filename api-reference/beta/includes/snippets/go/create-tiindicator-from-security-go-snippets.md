---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87408166c212995c6c1a12fd287c890a9f4a5a85
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989321"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTiIndicator()
action := "alert"
requestBody.SetAction(&action)
requestBody.SetActivityGroupNames( []string {
}
confidence := int32(0)
requestBody.SetConfidence(&confidence)
description := "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator."
requestBody.SetDescription(&description)
expirationDateTime, err := time.Parse(time.RFC3339, "2019-03-01T21:43:37.5031462+00:00")
requestBody.SetExpirationDateTime(&expirationDateTime)
externalId := "Test--8586509942679764298MS501"
requestBody.SetExternalId(&externalId)
fileHashType := "sha256"
requestBody.SetFileHashType(&fileHashType)
fileHashValue := "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313"
requestBody.SetFileHashValue(&fileHashValue)
requestBody.SetKillChain( []string {
}
requestBody.SetMalwareFamilyNames( []string {
}
severity := int32(0)
requestBody.SetSeverity(&severity)
requestBody.SetTags( []string {
}
targetProduct := "Azure Sentinel"
requestBody.SetTargetProduct(&targetProduct)
threatType := "WatchList"
requestBody.SetThreatType(&threatType)
tlpLevel := "green"
requestBody.SetTlpLevel(&tlpLevel)
options := &msgraphsdk.TiIndicatorsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Security().TiIndicators().Post(options)


```