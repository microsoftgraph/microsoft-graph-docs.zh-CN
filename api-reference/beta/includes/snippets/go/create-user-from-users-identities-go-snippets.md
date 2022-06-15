---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a755a1eb21a81683557f2ab170430e39848dd813
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098697"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUser()
displayName := "John Smith"
requestBody.SetDisplayName(&displayName)
requestBody.SetIdentities( []ObjectIdentity {
    msgraphsdk.NewObjectIdentity(),
signInType := "userName"
    SetSignInType(&signInType)
issuer := "contoso.onmicrosoft.com"
    SetIssuer(&issuer)
issuerAssignedId := "johnsmith"
    SetIssuerAssignedId(&issuerAssignedId)
    msgraphsdk.NewObjectIdentity(),
signInType := "emailAddress"
    SetSignInType(&signInType)
issuer := "contoso.onmicrosoft.com"
    SetIssuer(&issuer)
issuerAssignedId := "jsmith@yahoo.com"
    SetIssuerAssignedId(&issuerAssignedId)
    msgraphsdk.NewObjectIdentity(),
signInType := "federated"
    SetSignInType(&signInType)
issuer := "facebook.com"
    SetIssuer(&issuer)
issuerAssignedId := "5eecb0cd"
    SetIssuerAssignedId(&issuerAssignedId)
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