---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80bda49cc894041f229ad8d3ecb529f18c87516f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082759"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUser()
passwordProfile := msgraphsdk.NewPasswordProfile()
requestBody.SetPasswordProfile(passwordProfile)
forceChangePasswordNextSignIn := false
passwordProfile.SetForceChangePasswordNextSignIn(&forceChangePasswordNextSignIn)
password := "xWwvJ]6NMw+bWH-d"
passwordProfile.SetPassword(&password)
options := &msgraphsdk.UserRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Patch(options)


```