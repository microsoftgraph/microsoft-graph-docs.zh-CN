---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5690a4a93e6e8cfa38a9f44c9d2f15fe3f275e48
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087716"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeam()
requestBody.SetAdditionalData(map[string]interface{}{
    "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
    "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')",
}
options := &msgraphsdk.TeamsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Teams().Post(options)


```