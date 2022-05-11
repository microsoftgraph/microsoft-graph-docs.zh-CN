---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e7a9c3ef2fb0533dab56e11f4e5b95adbcf7b1b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328823"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CalendarViewRequestBuilderGetQueryParameters{
    StartDateTime: "2020-01-01T19:00:00-08:00",
    EndDateTime: "2020-01-02T19:00:00-08:00",
}
options := &msgraphsdk.CalendarViewRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Me().CalendarView().GetWithRequestConfigurationAndResponseHandler(options, nil)


```