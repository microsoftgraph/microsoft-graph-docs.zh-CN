---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4176eec460dc7033a320f49bd632f1d7f2f43643
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083292"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
linkedResourceId := "linkedResource-id"
graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).LinkedResourcesById(&linkedResourceId).Delete(options)


```