---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f16fe6fd9025758a5d0328720449423614351d9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098759"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
requestBody.SetAssignedLabels( []AssignedLabel {
    msgraphsdk.NewAssignedLabel(),
labelId := "45cd0c48-c540-4358-ad79-a3658cdc5b88"
    SetLabelId(&labelId)
}
groupId := "group-id"
graphClient.GroupsById(&groupId).Patch(requestBody)


```