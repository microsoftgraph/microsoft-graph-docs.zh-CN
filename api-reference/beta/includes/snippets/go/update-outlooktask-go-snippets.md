---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe1536d54cfab645725ac70fe15248e0ef8921e5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329265"
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
options := &msgraphsdk.OutlookTaskRequestBuilderPatchRequestConfiguration{
    Headers: headers,
}
outlookTaskId := "outlookTask-id"
graphClient.Me().Outlook().TasksById(&outlookTaskId).PatchWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```