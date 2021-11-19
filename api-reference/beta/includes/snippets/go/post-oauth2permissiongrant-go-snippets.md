---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6a286b0e85d0c74d97d520c5a4da3cf00dcee63
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102482"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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