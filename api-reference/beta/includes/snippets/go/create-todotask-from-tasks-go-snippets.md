---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b238ef570aa1e18e1ff0fbb4c5764b4bb964e2b8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088861"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTodoTask()
title := "A new task"
requestBody.SetTitle(&title)
requestBody.SetLinkedResources( []LinkedResource {
    msgraphsdk.NewLinkedResource(),
    SetAdditionalData(map[string]interface{}{
        "webUrl": "http://microsoft.com",
        "applicationName": "Microsoft",
        "displayName": "Microsoft",
    }
}
options := &msgraphsdk.TasksRequestBuilderPostOptions{
    Body: requestBody,
}
todoTaskListId := "todoTaskList-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).Tasks().Post(options)


```