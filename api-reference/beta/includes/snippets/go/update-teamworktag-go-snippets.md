---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84a0d5c28e500404e5e249923c0c3aec349aee4d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017736"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTeamworkTag()
displayName := "Finance"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.TeamworkTagRequestBuilderPatchOptions{
    Body: requestBody,
}
teamId := "team-id"
teamworkTagId := "teamworkTag-id"
graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).Patch(options)


```