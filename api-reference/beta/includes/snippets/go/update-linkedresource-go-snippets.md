---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 283c35c6583cc9724bd99d7b93b2c34f1cd3938d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412245"
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
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).LinkedResourcesById(&linkedResourceId).Patch(options)


```