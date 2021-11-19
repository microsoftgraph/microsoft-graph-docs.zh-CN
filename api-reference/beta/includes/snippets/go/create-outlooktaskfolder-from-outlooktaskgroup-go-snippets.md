---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3f130ca689f712533592bbb011eb163fe958bdb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097972"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTaskFolder()
name := "Cooking"
requestBody.SetName(&name)
options := &msgraphsdk.TaskFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
outlookTaskGroupId := "outlookTaskGroup-id"
result, err := graphClient.Me().Outlook().TaskGroupsById(&outlookTaskGroupId).TaskFolders().Post(options)


```