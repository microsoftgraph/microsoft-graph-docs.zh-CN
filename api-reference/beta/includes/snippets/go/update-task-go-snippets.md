---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ce28c253b0449cb4fbc60a860894bd766782503
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327176"
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
printTaskDefinitionId := "printTaskDefinition-id"
printTaskId := "printTask-id"
graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).TasksById(&printTaskId).Patch(requestBody)


```