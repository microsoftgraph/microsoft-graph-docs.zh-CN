---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8330c2d46181aebbf2920972a7452026624ec026
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032058"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSchedulingGroup()
displayName := "Cashiers"
requestBody.SetDisplayName(&displayName)
isActive := true
requestBody.SetIsActive(&isActive)
requestBody.SetUserIds( []String {
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851",
}
options := &msgraphsdk.SchedulingGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SchedulingGroups().Post(options)


```