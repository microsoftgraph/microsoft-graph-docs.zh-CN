---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c46be84da61b81ee6d81eade5bf8d32813f17de7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974983"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.CalendarViewRequestBuilderGetQueryParameters{
    StartDateTime: "2017-01-01T19:00:00-08:00",
    EndDateTime: "2017-10-01T19:00:00.00-08:00",
}
headers := map[string]string{
    "Prefer": "outlook.body-content-type="text""
}
options := &msgraphsdk.CalendarViewRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).CalendarView().Get(options)


```