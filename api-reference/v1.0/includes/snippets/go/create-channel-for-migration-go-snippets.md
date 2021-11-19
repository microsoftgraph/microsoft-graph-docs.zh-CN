---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ad141c9f68e4728fdaff1ed749280176c7accdb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099739"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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