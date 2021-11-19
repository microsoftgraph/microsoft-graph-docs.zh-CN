---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 953b5e03b078359e9712d93a36dcd99daf1a1aee
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097867"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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