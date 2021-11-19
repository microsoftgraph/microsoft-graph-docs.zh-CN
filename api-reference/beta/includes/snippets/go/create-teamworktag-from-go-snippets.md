---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d99e988aad8eb304405f945386ca0c21a2fbf8e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088337"
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
options := &msgraphsdk.TagsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Tags().Post(options)


```