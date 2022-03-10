---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b58e9953231c42763b61397bda802b9ff06ac973
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412266"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
reason := "none"
requestBody.SetReason(&reason)
options := &msgraphsdk.RejectRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).Reject(call-id).Post(options)


```