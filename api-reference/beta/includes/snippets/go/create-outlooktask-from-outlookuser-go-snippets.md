---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2cb578c74242fee0b51ad06429b13d94d73b3f4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090047"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTask()
subject := "Shop for children's weekend"
requestBody.SetSubject(&subject)
startDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStartDateTime(startDateTime)
dateTime := "2016-05-03T09:00:00"
startDateTime.SetDateTime(&dateTime)
timeZone := "Eastern Standard Time"
startDateTime.SetTimeZone(&timeZone)
dueDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetDueDateTime(dueDateTime)
dateTime := "2016-05-05T16:00:00"
dueDateTime.SetDateTime(&dateTime)
timeZone := "Eastern Standard Time"
dueDateTime.SetTimeZone(&timeZone)
headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.TasksRequestBuilderPostOptions{
    Body: requestBody,
    H: headers,
}
result, err := graphClient.Me().Outlook().Tasks().Post(options)


```