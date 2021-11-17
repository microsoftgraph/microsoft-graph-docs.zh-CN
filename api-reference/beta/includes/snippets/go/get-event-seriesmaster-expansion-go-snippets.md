---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1782e90a184cfd6eeb11622661c29071e3472867
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028585"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.EventRequestBuilderGetQueryParameters{
    Select: "subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences$expand",
}
options := &msgraphsdk.EventRequestBuilderGetOptions{
    Q: requestParameters,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Get(options)


```