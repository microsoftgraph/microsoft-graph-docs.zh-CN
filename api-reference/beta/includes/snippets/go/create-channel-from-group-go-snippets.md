---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20b377289626f30ea5ca1d0e6611fce2aed9dac4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091082"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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