---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5c802aa936b9c8daec2d6ac884479e47614ec11
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081909"
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
graphClient.Communications().CallsById(&callId).Reject().Post(options)


```