---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cda29ed2e0a6407a77e456be0cb1da3c4909f07
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097368"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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