---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7927e696148f413ceb6dc5e72183f5d70811c3c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316137"
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
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Post(requestBody)


```