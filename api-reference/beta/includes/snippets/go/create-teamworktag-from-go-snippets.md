---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d6b0359f09eb442f28452533ded149def066280
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098810"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeamworkTag()
displayName := "Finance"
requestBody.SetDisplayName(&displayName)
requestBody.SetMembers( []TeamworkTagMember {
    msgraphsdk.NewTeamworkTagMember(),
userId := "92f6952f-61ca-4a94-8910-508a240bc167"
    SetUserId(&userId)
    msgraphsdk.NewTeamworkTagMember(),
userId := "085d800c-b86b-4bfc-a857-9371ad1caf29"
    SetUserId(&userId)
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Tags().Post(requestBody)


```