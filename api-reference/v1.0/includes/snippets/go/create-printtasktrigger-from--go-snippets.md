---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1487943c42a7b1eeea899687af933e595fcd710
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082973"
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
options := &msgraphsdk.TaskTriggersRequestBuilderPostOptions{
    Body: requestBody,
}
printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).TaskTriggers().Post(options)


```