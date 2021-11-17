---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b06f7fb98f0cc994dbb49bf048293de2733cbac
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028565"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
comment := "Cancelling for this week due to all hands"
requestBody.SetComment(&comment)
options := &msgraphsdk.CancelRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Cancel().Post(options)


```