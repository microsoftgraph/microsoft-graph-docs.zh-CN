---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 433a49177a34171c4258ada82770a08774d6df2f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106968"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBaseTask()
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
body.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.itemBody",
}
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
personalProperties := msgraphsdk.NewPersonalTaskProperties()
requestBody.SetPersonalProperties(personalProperties)
personalProperties.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.personalTaskProperties",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.baseTask",
}
options := &msgraphsdk.BaseTaskRequestBuilderPatchOptions{
    Body: requestBody,
}
baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).Patch(options)


```