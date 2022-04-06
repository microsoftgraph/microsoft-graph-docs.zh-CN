---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1636d9dab5f932946dfcb9520761677f435b704
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528145"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBaseTaskList()
displayName := "Shopping list"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.taskList",
}
options := &msgraphsdk.ListsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Tasks().Lists().Post(options)


```