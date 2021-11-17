---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e71631ed60543dd2a6a9decc0f9f344f5cce73c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034356"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
memberId := "319b41e8-d9e4-42f8-bdc9-741113f48b33"
requestBody.SetMemberId(&memberId)
membershipRule := "(user.displayName -startsWith "EndTestUser")"
requestBody.SetMembershipRule(&membershipRule)
options := &msgraphsdk.EvaluateDynamicMembershipRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Groups().EvaluateDynamicMembership().Post(options)


```