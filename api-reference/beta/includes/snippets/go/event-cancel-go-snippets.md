---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba90c16bf7c9ba509cb0f6d09a64fcaee0fcbaa6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082226"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
comment := "Cancelling for this week due to all hands"
requestBody.SetComment(&comment)
options := &msgraphsdk.CancelRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Cancel().Post(options)


```