---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b41ce1d3f91c862a639de5140c7eacb38c16478
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978156"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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