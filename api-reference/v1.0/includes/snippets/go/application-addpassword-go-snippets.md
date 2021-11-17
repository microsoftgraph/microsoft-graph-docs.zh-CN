---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a93122ccc494b5fd51f5192c163d80a83c1080dd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979626"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
passwordCredential := msgraphsdk.NewPasswordCredential()
requestBody.SetPasswordCredential(passwordCredential)
displayName := "Password friendly name"
passwordCredential.SetDisplayName(&displayName)
options := &msgraphsdk.AddPasswordRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).AddPassword().Post(options)


```