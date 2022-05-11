---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c994f39605817ae8e0966bb319cf4d9dc64dac95
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325874"
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
result, err := graphClient.Users().Post(requestBody)


```