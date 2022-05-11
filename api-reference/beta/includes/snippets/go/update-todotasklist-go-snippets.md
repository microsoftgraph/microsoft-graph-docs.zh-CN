---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b563ff4b2236881474f303f649be457caf5d09b0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327419"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTodoTaskList()
displayName := "Vacation Plan"
requestBody.SetDisplayName(&displayName)
todoTaskListId := "todoTaskList-id"
graphClient.Me().Todo().ListsById(&todoTaskListId).Patch(requestBody)


```