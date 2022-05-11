---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 043836f99bea54edd931c15470a3e8a87b4f0049
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329108"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CalendarViewRequestBuilderGetQueryParameters{
    StartDateTime: "2017-01-01T19:00:00-08:00",
    EndDateTime: "2017-10-01T19:00:00.00-08:00",
}
headers := map[string]string{
    "Prefer": "outlook.body-content-type="text""
}
options := &msgraphsdk.CalendarViewRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).CalendarView().GetWithRequestConfigurationAndResponseHandler(options, nil)


```