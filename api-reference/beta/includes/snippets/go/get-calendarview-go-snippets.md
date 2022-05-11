---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e3387c04286fd501fdc0afc3ecbbe84cae74350
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328169"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CalendarViewRequestBuilderGetQueryParameters{
    StartDateTime: "2017-01-01T19:00:00-08:00",
    EndDateTime: "2017-01-07T19:00:00-08:00",
}
options := &msgraphsdk.CalendarViewRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Me().Calendar().CalendarView().GetWithRequestConfigurationAndResponseHandler(options, nil)


```