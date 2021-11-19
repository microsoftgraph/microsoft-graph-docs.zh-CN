---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0512d3757a8adc8ef531f5c4b59101a6b7161d5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092298"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTaskFolder()
name := "Volunteer"
requestBody.SetName(&name)
options := &msgraphsdk.TaskFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Outlook().TaskFolders().Post(options)


```