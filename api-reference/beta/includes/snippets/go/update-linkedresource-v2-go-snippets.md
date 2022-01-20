---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54501359946ccb2a6ce3eac5354f6bece9f946f5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089920"
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
graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).LinkedResourcesById(&linkedResource_v2Id).Patch(options)


```