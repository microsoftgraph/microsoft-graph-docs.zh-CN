---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 097481f409ce1636ca5245f92d06766347a30856
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081866"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewLinkedResource()
webUrl := "http://microsoft.com"
requestBody.SetWebUrl(&webUrl)
applicationName := "Microsoft"
requestBody.SetApplicationName(&applicationName)
displayName := "Microsoft"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.linkedResource",
}
options := &msgraphsdk.LinkedResourceRequestBuilderPatchOptions{
    Body: requestBody,
}
todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
linkedResourceId := "linkedResource-id"
graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).LinkedResourcesById(&linkedResourceId).Patch(options)


```