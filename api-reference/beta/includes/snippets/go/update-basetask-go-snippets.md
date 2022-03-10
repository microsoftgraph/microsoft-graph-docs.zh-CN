---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b1fa89cf9f6c3f46b1c60ada5ed158ffc798bdb
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411820"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBaseTask()
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
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.baseTask",
}
options := &msgraphsdk.BaseTaskRequestBuilderPatchOptions{
    Body: requestBody,
}
baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).Patch(options)


```