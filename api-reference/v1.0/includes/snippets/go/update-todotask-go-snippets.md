---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5675e44c4807e6748419cd2d8fe466ae3e862d88
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029070"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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