---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7e28fbf4bb26afa3a1c7c791f1d653d6efaf494
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326258"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
outlookTaskFolderId := "outlookTaskFolder-id"
result, err := graphClient.Me().Outlook().TaskFoldersById(&outlookTaskFolderId).Tasks().Post(requestBody)


```