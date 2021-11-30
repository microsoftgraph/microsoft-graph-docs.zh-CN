---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce532af0b0821599b0f18544873b3c8cf8cd51f0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226206"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewServicePrincipal()
customSecurityAttributes := msgraphsdk.NewCustomSecurityAttributeValue()
requestBody.SetCustomSecurityAttributes(customSecurityAttributes)
customSecurityAttributes.SetAdditionalData(map[string]interface{}{
}
options := &msgraphsdk.ServicePrincipalRequestBuilderPatchOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).Patch(options)


```