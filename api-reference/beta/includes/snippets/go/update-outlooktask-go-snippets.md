---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a97f72e44a42e970ab7263143a1d9b5a88e8eb4a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097025"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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