---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ff0b5ff916c53427cf02ffd6bb8393021209cf5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUser()
accountEnabled := true
requestBody.SetAccountEnabled(&accountEnabled)
displayName := "Adele Vance"
requestBody.SetDisplayName(&displayName)
mailNickname := "AdeleV"
requestBody.SetMailNickname(&mailNickname)
userPrincipalName := "AdeleV@contoso.onmicrosoft.com"
requestBody.SetUserPrincipalName(&userPrincipalName)
passwordProfile := msgraphsdk.NewPasswordProfile()
requestBody.SetPasswordProfile(passwordProfile)
forceChangePasswordNextSignIn := true
passwordProfile.SetForceChangePasswordNextSignIn(&forceChangePasswordNextSignIn)
password := "xWwvJ]6NMw+bWH-d"
passwordProfile.SetPassword(&password)
options := &msgraphsdk.UsersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Users().Post(options)


```