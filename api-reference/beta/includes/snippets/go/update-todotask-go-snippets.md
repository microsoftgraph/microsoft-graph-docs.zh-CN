---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 243c681203817938115d6b8fe864e6cd4a008ad6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101256"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTodoTask()
dueDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetDueDateTime(dueDateTime)
dateTime := "2020-07-25T16:00:00"
dueDateTime.SetDateTime(&dateTime)
timeZone := "Eastern Standard Time"
dueDateTime.SetTimeZone(&timeZone)
options := &msgraphsdk.TodoTaskRequestBuilderPatchOptions{
    Body: requestBody,
}
todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).Patch(options)


```