---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08179a803031ebdec8f11b5c5137de35425566cb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087830"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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