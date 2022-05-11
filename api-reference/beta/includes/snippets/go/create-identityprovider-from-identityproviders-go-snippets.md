---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57c5e9bcc8e50e46a2b6832388b6d0897228b76d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328151"
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
result, err := graphClient.IdentityProviders().Post(requestBody)


```