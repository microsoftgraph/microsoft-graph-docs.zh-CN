---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c057034836c8fee5d013aab854b5a6ff0940ea3b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085019"
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
options := &msgraphsdk.CalendarViewRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).CalendarView().Get(options)


```