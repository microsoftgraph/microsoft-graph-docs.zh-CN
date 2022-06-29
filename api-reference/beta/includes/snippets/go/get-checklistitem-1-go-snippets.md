---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ac7b70c7db543a24241d241ed7da38bccebbfa4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66440748"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
checklistItemId := "checklistItem-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).ChecklistItemsById(&checklistItemId).Get()


```