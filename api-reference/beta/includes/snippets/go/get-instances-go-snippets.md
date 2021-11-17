---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1364d90ae95b9bdbb9e36885c3c35e2d73557f52
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032464"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.InstancesRequestBuilderGetQueryParameters{
    StartDateTime: "2019-04-08T09:00:00.0000000",
    EndDateTime: "2019-04-30T09:00:00.0000000",
    Select: "subject,bodyPreview,seriesMasterId,type,recurrence,start,end",
}
options := &msgraphsdk.InstancesRequestBuilderGetOptions{
    Q: requestParameters,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Instances().Get(options)


```