---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13b3b4e53670d38fcea294568db7c8c8026b8f57
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006884"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewChannel()
displayName := "Import_150958_99z"
requestBody.SetDisplayName(&displayName)
description := "Import_150958_99z"
requestBody.SetDescription(&description)
createdDateTime, err := time.Parse(time.RFC3339, "2020-03-14T11:22:17.067Z")
requestBody.SetCreatedDateTime(&createdDateTime)
requestBody.SetAdditionalData(map[string]interface{}{
    "@microsoft.graph.channelCreationMode": "migration",
}
options := &msgraphsdk.ChannelsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Post(options)


```