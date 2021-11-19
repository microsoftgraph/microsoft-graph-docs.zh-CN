---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f77a9d90e3737fd5411e0c6fae347d5f6d0c7707
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092154"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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