---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec84f489e7961b2a7e80e8b66bc82756a46418aa
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327120"
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
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SchedulingGroups().Post(requestBody)


```