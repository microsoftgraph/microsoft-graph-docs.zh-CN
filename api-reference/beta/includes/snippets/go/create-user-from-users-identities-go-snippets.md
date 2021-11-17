---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3451f72a2ba7ee9278c86f4224ba7a08380a0712
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985052"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUser()
displayName := "John Smith"
requestBody.SetDisplayName(&displayName)
requestBody.SetIdentities( []ObjectIdentity {
    msgraphsdk.NewObjectIdentity(),
    SetAdditionalData(map[string]interface{}{
        "signInType": "userName",
        "issuer": "contoso.onmicrosoft.com",
        "issuerAssignedId": "johnsmith",
    }
    msgraphsdk.NewObjectIdentity(),
    SetAdditionalData(map[string]interface{}{
        "signInType": "emailAddress",
        "issuer": "contoso.onmicrosoft.com",
        "issuerAssignedId": "jsmith@yahoo.com",
    }
    msgraphsdk.NewObjectIdentity(),
    SetAdditionalData(map[string]interface{}{
        "signInType": "federated",
        "issuer": "facebook.com",
        "issuerAssignedId": "5eecb0cd",
    }
}
passwordProfile := msgraphsdk.NewPasswordProfile()
requestBody.SetPasswordProfile(passwordProfile)
password := "password-value"
passwordProfile.SetPassword(&password)
forceChangePasswordNextSignIn := false
passwordProfile.SetForceChangePasswordNextSignIn(&forceChangePasswordNextSignIn)
passwordPolicies := "DisablePasswordExpiration"
requestBody.SetPasswordPolicies(&passwordPolicies)
options := &msgraphsdk.UsersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Users().Post(options)


```