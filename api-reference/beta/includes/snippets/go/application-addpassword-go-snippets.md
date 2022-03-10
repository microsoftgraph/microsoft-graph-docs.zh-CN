---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10655e41236575d28b6793a7d559673323d081c7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411837"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPasswordCredentialRequestBody()
passwordCredential := msgraphsdk.NewPasswordCredential()
requestBody.SetPasswordCredential(passwordCredential)
displayName := "Password friendly name"
passwordCredential.SetDisplayName(&displayName)
options := &msgraphsdk.AddPasswordRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).AddPassword(application-id).Post(options)


```