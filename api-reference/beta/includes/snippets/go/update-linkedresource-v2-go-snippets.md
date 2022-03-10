---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da8a2fe4b059538cb021ceb691c8f5cc313a7fee
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411905"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewLinkedResource_v2()
webUrl := "https://microsoft.com"
requestBody.SetWebUrl(&webUrl)
applicationName := "Microsoft"
requestBody.SetApplicationName(&applicationName)
displayName := "Microsoft Web page"
requestBody.SetDisplayName(&displayName)
externalId := "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
requestBody.SetExternalId(&externalId)
options := &msgraphsdk.LinkedResource_v2RequestBuilderPatchOptions{
    Body: requestBody,
}
baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
linkedResource_v2Id := "linkedResource_v2-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).LinkedResourcesById(&linkedResource_v2Id).Patch(options)


```