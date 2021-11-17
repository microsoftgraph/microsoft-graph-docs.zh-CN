---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b482552cdbd376dced6b3e2b0e5c49cf2b208582
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979522"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
reason := "busy"
requestBody.SetReason(&reason)
options := &msgraphsdk.RejectRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).Reject().Post(options)


```