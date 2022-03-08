---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e12029d554b528be84b2c80b30a86e1e411786d7
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336121"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventRequestBuilderGetQueryParameters{
    Select: "subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences",
    Expand: "exceptionOccurrences",
}
options := &msgraphsdk.EventRequestBuilderGetOptions{
    Q: requestParameters,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Get(options)


```