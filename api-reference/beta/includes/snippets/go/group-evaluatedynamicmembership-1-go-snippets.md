---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c85721c56ac3d2ae4636b5a5a6112562b6c932c5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093014"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
memberId := "319b41e8-d9e4-42f8-bdc9-741113f48b33"
requestBody.SetMemberId(&memberId)
options := &msgraphsdk.EvaluateDynamicMembershipRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).EvaluateDynamicMembership().Post(options)


```