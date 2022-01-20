---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3bd734deb1b61b1abebe041e56383662b3714ad
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090796"
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
graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).ChecklistItemsById(&checklistItemId).Patch(options)


```