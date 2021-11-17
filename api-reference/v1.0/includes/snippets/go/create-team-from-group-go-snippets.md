---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6656de3e20ca57e7795bdd91319ccc9dbe813dd2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029303"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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