---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e4bf992a9ff636d23f7e2a0ca750470d50da227
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528078"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBaseTask()
textBody := "String"
requestBody.SetTextBody(&textBody)
bodyLastModifiedDateTime, err := time.Parse(time.RFC3339, "String (timestamp)")
requestBody.SetBodyLastModifiedDateTime(&bodyLastModifiedDateTime)
completedDateTime, err := time.Parse(time.RFC3339, "String (timestamp)")
requestBody.SetCompletedDateTime(&completedDateTime)
dueDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetDueDateTime(dueDateTime)
dueDateTime.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
}
startDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStartDateTime(startDateTime)
startDateTime.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
}
importance := "String"
requestBody.SetImportance(&importance)
recurrence := msgraphsdk.NewPatternedRecurrence()
requestBody.SetRecurrence(recurrence)
recurrence.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.patternedRecurrence",
}
displayName := "String"
requestBody.SetDisplayName(&displayName)
status := "String"
requestBody.SetStatus(&status)
viewpoint := msgraphsdk.NewTaskViewpoint()
requestBody.SetViewpoint(viewpoint)
viewpoint.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.taskViewpoint",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.task",
}
options := &msgraphsdk.TasksRequestBuilderPostOptions{
    Body: requestBody,
}
baseTaskListId := "baseTaskList-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).Tasks().Post(options)


```