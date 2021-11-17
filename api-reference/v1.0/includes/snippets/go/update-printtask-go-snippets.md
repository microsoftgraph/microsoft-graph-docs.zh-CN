---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5944ee904de4a99df708d585e97baeec04219ec0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983869"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPrintTask()
status := msgraphsdk.NewPrintTaskStatus()
requestBody.SetStatus(status)
state := "completed"
status.SetState(&state)
description := "completed"
status.SetDescription(&description)
options := &msgraphsdk.PrintTaskRequestBuilderPatchOptions{
    Body: requestBody,
}
printTaskDefinitionId := "printTaskDefinition-id"
printTaskId := "printTask-id"
graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).TasksById(&printTaskId).Patch(options)


```