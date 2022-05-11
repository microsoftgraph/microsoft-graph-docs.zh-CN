---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9015206ff5e65fbcc1bcf9565324603000564bc4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326772"
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
todoTaskListId := "todoTaskList-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).Tasks().Post(requestBody)


```