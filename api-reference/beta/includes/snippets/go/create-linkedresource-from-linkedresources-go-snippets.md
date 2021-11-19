---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5105f63a4b03321c3e5d9f74d7e0f397610e2ec9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083752"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewLinkedResource()
webUrl := "https://microsoft.com"
requestBody.SetWebUrl(&webUrl)
applicationName := "Microsoft"
requestBody.SetApplicationName(&applicationName)
displayName := "Microsoft"
requestBody.SetDisplayName(&displayName)
externalId := "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
requestBody.SetExternalId(&externalId)
options := &msgraphsdk.LinkedResourcesRequestBuilderPostOptions{
    Body: requestBody,
}
todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).LinkedResources().Post(options)


```