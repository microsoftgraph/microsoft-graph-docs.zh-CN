---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c564068f8b13198da90dfdad894c63ad8d0bec02
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979549"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAuthenticationMethodsPolicy()
requestBody.SetAuthenticationMethodConfigurations( []AuthenticationMethodConfiguration {
    msgraphsdk.NewAuthenticationMethodConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
        "id": "Fido2",
        "state": "disabled",
        "isSelfServiceRegistrationAllowed": false,
        "isAttestationEnforced": false,
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy",
}
options := &msgraphsdk.AuthenticationMethodsPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().AuthenticationMethodsPolicy().Patch(options)


```