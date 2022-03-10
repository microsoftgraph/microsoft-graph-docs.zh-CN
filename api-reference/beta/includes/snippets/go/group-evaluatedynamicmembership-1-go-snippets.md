---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 923769ea3d4c2ced3eae1e12a0528b8e598e09d1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412624"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMemberIdRequestBody()
memberId := "319b41e8-d9e4-42f8-bdc9-741113f48b33"
requestBody.SetMemberId(&memberId)
options := &msgraphsdk.EvaluateDynamicMembershipRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).EvaluateDynamicMembership(group-id).Post(options)


```