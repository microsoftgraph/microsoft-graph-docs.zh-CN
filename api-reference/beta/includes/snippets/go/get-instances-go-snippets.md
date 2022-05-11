---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddcd353e868a71ad5ce63b67621ca642491b3878
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327275"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.InstancesRequestBuilderGetQueryParameters{
    StartDateTime: "2019-04-08T09:00:00.0000000",
    EndDateTime: "2019-04-30T09:00:00.0000000",
    Select: "subject,bodyPreview,seriesMasterId,type,recurrence,start,end",
}
options := &msgraphsdk.InstancesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Instances().GetWithRequestConfigurationAndResponseHandler(options, nil)


```