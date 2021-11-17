---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5596025633665ef80e24eb6fb8b2d6c0ea84487
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021754"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOAuth2PermissionGrant()
clientId := "clientId-value"
requestBody.SetClientId(&clientId)
consentType := "consentType-value"
requestBody.SetConsentType(&consentType)
principalId := "principalId-value"
requestBody.SetPrincipalId(&principalId)
resourceId := "resourceId-value"
requestBody.SetResourceId(&resourceId)
scope := "scope-value"
requestBody.SetScope(&scope)
startTime, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
requestBody.SetStartTime(&startTime)
expiryTime, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
requestBody.SetExpiryTime(&expiryTime)
options := &msgraphsdk.Oauth2PermissionGrantsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Oauth2PermissionGrants().Post(options)


```