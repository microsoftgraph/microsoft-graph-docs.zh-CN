---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c87e8a422c56b07e28cb1330e0931073eb5115b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328991"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeamworkTag()
displayName := "Finance"
requestBody.SetDisplayName(&displayName)
requestBody.SetMembers( []TeamworkTagMember {
    msgraphsdk.NewTeamworkTagMember(),
    SetAdditionalData(map[string]interface{}{
        "userId": "92f6952f-61ca-4a94-8910-508a240bc167",
    }
    msgraphsdk.NewTeamworkTagMember(),
    SetAdditionalData(map[string]interface{}{
        "userId": "085d800c-b86b-4bfc-a857-9371ad1caf29",
    }
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Tags().Post(requestBody)


```