---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e025886376166b1f34fc6207a6700be65d052670
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411628"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
isRead := true
requestBody.SetIsRead(&isRead)
options := &msgraphsdk.MessageRequestBuilderPatchOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Patch(options)


```