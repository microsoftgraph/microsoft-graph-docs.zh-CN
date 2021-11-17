---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1fb3e66940ddaccc0afdea780ca43209a3aa3e0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977238"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).Delete(options)


```