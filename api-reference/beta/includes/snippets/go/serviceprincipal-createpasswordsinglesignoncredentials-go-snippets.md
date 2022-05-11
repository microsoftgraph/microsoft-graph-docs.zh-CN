---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23d2656f9ebc8ef682466d5573b6ed9a54f6439e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328591"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
id := "5793aa3b-cca9-4794-679a240f8b58"
requestBody.SetId(&id)
requestBody.SetCredentials( []Credential {
    msgraphsdk.NewCredential(),
    SetAdditionalData(map[string]interface{}{
        "fieldId": "param_username",
        "value": "myusername",
        "type": "username",
    }
    msgraphsdk.NewCredential(),
    SetAdditionalData(map[string]interface{}{
        "fieldId": "param_password",
        "value": "pa$$w0rd",
        "type": "password",
    }
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).CreatePasswordSingleSignOnCredentials(servicePrincipal-id).Post(requestBody)


```