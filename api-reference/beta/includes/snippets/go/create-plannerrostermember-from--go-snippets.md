---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6b37170bfaf66a738e1f448da42cbe27416edd9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990057"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPlannerRosterMember()
userId := "String"
requestBody.SetUserId(&userId)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.plannerRosterMember",
}
options := &msgraphsdk.MembersRequestBuilderPostOptions{
    Body: requestBody,
}
plannerRosterId := "plannerRoster-id"
result, err := graphClient.Planner().RostersById(&plannerRosterId).Members().Post(options)


```