---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaeafda61ddaced303cdc8f1492bd3ff1839f8c3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412751"
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
options := &msgraphsdk.CreatePasswordSingleSignOnCredentialsRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).CreatePasswordSingleSignOnCredentials(servicePrincipal-id).Post(options)


```