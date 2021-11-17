---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fa3861338b0284b6aa8277522868af6e1f0ce07
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011359"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOutlookTask()
subject := "Shop for dinner"
requestBody.SetSubject(&subject)
startDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStartDateTime(startDateTime)
dateTime := "2016-04-23T18:00:00"
startDateTime.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
startDateTime.SetTimeZone(&timeZone)
dueDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetDueDateTime(dueDateTime)
dateTime := "2016-04-25T13:00:00"
dueDateTime.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
dueDateTime.SetTimeZone(&timeZone)
options := &msgraphsdk.TasksRequestBuilderPostOptions{
    Body: requestBody,
}
outlookTaskFolderId := "outlookTaskFolder-id"
result, err := graphClient.Me().Outlook().TaskFoldersById(&outlookTaskFolderId).Tasks().Post(options)


```