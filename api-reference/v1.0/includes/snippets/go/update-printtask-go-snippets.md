---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b92d07859f2de85842d19a522ee782675c935b0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094370"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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