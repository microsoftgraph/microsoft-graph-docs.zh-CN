---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8319cdb810ed0986c431cd81478489f9c8e8eba
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328039"
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
result, err := graphClient.Oauth2PermissionGrants().Post(requestBody)


```