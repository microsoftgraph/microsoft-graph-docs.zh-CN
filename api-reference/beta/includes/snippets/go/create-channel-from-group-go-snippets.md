---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f208dd8c63c998686dba40dc3da3f8ec98e5c43f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990361"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewChannel()
displayName := "Architecture Discussion"
requestBody.SetDisplayName(&displayName)
description := "This channel is where we debate all future architecture plans"
requestBody.SetDescription(&description)
membershipType := "standard"
requestBody.SetMembershipType(&membershipType)
options := &msgraphsdk.ChannelsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Post(options)


```