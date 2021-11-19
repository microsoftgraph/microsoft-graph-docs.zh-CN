---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61c2dc3ea09611e4484d3a904b6070c819f25542
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091628"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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