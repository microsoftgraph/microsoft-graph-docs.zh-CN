---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65c4ac15b8aca7e50437abc23df3ad3755dd08bd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997295"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPrintTaskTrigger()
event := "jobStarted"
requestBody.SetEvent(&event)
requestBody.SetAdditionalData(map[string]interface{}{
    "definition@odata.bind": "https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c",
}
options := &msgraphsdk.TaskTriggersRequestBuilderPostOptions{
    Body: requestBody,
}
printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).TaskTriggers().Post(options)


```