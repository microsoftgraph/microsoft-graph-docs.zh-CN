---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb1c8819aa583a57723d73220593266a8ebdec7f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412392"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChecklistItem()
displayName := "buy cake"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ChecklistItemRequestBuilderPatchOptions{
    Body: requestBody,
}
baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
checklistItemId := "checklistItem-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).ChecklistItemsById(&checklistItemId).Patch(options)


```