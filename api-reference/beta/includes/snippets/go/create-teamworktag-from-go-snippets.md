---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb65c6505561d6eb9ea8123cba8f544a2e634e9a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017778"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.TagsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Tags().Post(options)


```