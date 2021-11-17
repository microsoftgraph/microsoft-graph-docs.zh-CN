---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e14a95bf1d1921b98d928ff626ff5b275e74e23c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011568"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOutlookTask()
dueDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetDueDateTime(dueDateTime)
dateTime := "2016-05-06T16:00:00"
dueDateTime.SetDateTime(&dateTime)
timeZone := "Eastern Standard Time"
dueDateTime.SetTimeZone(&timeZone)
headers := map[string]string{
    "Prefer": "outlook.timezone="Eastern Standard Time""
}
options := &msgraphsdk.OutlookTaskRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
outlookTaskId := "outlookTask-id"
graphClient.Me().Outlook().TasksById(&outlookTaskId).Patch(options)


```