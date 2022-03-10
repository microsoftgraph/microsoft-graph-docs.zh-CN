---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a41a1cf666bc7bf6befa49110dfc58f9e9b4697a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411883"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewRoleRequestBody()
role := "viewer"
requestBody.SetRole(&role)
options := &msgraphsdk.ChangeScreenSharingRoleRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).ChangeScreenSharingRole(call-id).Post(options)


```