---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e16b1891b06983db55b90535881c871614a17390
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086691"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeam()
displayName := "My Sample Team"
requestBody.SetDisplayName(&displayName)
description := "My Sample Team’s Description"
requestBody.SetDescription(&description)
requestBody.SetAdditionalData(map[string]interface{}{
    "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
}
options := &msgraphsdk.TeamsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Teams().Post(options)


```