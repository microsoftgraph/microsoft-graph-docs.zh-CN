---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4672755db91e4d44aa2f74d3f502b1519a9e69ba
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327403"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
channelId := "channel-id"
conversationMemberId := "conversationMember-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).MembersById(&conversationMemberId).Get()


```