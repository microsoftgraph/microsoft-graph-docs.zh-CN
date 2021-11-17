---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbb7fce19c670b8bafee779f6f237361b93d0a25
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033766"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.UpdatePasswordSingleSignOnCredentialsRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).UpdatePasswordSingleSignOnCredentials().Post(options)


```