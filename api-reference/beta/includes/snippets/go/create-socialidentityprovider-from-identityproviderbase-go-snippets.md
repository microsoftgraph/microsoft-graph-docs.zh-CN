---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d49f9f6515a036d229536f017d26d5b77f675aed
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100073"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProviderBase()
displayName := "Login with Amazon"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.socialIdentityProvider",
    "identityProviderType": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000",
}
options := &msgraphsdk.IdentityProvidersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().IdentityProviders().Post(options)


```