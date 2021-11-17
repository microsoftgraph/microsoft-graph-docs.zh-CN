---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 831c199aa85ad594f387438d7e5c93cf8c89acd6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017645"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTeamworkTagMember()
userId := "97f62344-57dc-409c-88ad-c4af14158ff5"
requestBody.SetUserId(&userId)
options := &msgraphsdk.MembersRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
teamworkTagId := "teamworkTag-id"
result, err := graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).Members().Post(options)


```