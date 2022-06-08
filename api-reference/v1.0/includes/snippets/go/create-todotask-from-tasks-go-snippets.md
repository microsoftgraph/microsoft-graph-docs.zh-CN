---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4731d8353086d2fb71e123b7569e738ad59a7838
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946812"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTodoTask()
title := "A new task"
requestBody.SetTitle(&title)
requestBody.SetCategories( []String {
    "Important",
}
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