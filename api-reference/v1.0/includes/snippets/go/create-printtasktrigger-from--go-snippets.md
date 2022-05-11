---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53f36eeb3ab301435c81a4c0fef732c69796aa09
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326613"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrintTaskTrigger()
event := "jobStarted"
requestBody.SetEvent(&event)
requestBody.SetAdditionalData(map[string]interface{}{
    "definition@odata.bind": "https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}",
}
printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).TaskTriggers().Post(requestBody)


```