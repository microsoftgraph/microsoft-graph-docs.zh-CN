---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1a0ffc14f69d49233a1afc1b23d2e171b3657a1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327531"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOAuth2PermissionGrant()
clientId := "ef969797-201d-4f6b-960c-e9ed5f31dab5"
requestBody.SetClientId(&clientId)
consentType := "AllPrincipals"
requestBody.SetConsentType(&consentType)
resourceId := "943603e4-e787-4fe9-93d1-e30f749aae39"
requestBody.SetResourceId(&resourceId)
scope := "DelegatedPermissionGrant.ReadWrite.All"
requestBody.SetScope(&scope)
startTime, err := time.Parse(time.RFC3339, "2022-03-17T00:00:00Z")
requestBody.SetStartTime(&startTime)
expiryTime, err := time.Parse(time.RFC3339, "2023-03-17T00:00:00Z")
requestBody.SetExpiryTime(&expiryTime)
result, err := graphClient.Oauth2PermissionGrants().Post(requestBody)


```