---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed16847380e94e057492436f7bd84cda751d437c
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66440759"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
checklistItemId := "checklistItem-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).ChecklistItemsById(&checklistItemId).Get()


```