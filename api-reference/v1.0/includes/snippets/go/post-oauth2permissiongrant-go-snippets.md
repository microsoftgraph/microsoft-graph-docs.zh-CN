---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cf421ac9b9bcf09318b5ed3e6a7a444b2f2c2ad
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758635"
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
options := &msgraphsdk.Oauth2PermissionGrantsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Oauth2PermissionGrants().Post(options)


```