---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: deae1d752c5f77d702022952f7c24074ce6f1659
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66436234"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChecklistItem()
displayName := "buy cake"
requestBody.SetDisplayName(&displayName)
todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
checklistItemId := "checklistItem-id"
graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).ChecklistItemsById(&checklistItemId).Patch(requestBody)


```