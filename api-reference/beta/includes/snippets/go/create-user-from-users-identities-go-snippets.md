---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2013fb478b878e77a386c5c11e5338249094b4a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089805"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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