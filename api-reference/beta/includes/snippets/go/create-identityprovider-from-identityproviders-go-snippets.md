---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 528e70ea84bb072c008befbb429468639308feab
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096601"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProvider()
name := "Login with Amazon"
requestBody.SetName(&name)
type := "Amazon"
requestBody.SetType(&type)
clientId := "56433757-cadd-4135-8431-2c9e3fd68ae8"
requestBody.SetClientId(&clientId)
clientSecret := "000000000000"
requestBody.SetClientSecret(&clientSecret)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.identityProvider",
}
options := &msgraphsdk.IdentityProvidersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityProviders().Post(options)


```