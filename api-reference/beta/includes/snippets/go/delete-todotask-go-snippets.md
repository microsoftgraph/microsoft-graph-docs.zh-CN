---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23cccbe322d04b3894b4742ebf5de4b051aa3730
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325760"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).Delete()


```