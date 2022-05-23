---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4df210779d2e611dfe72f532c7d1e0b3215da7e
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628959"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
channelId := "channel-id"
sharedWithChannelTeamInfoId := "sharedWithChannelTeamInfo-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).SharedWithTeamsById(&sharedWithChannelTeamInfoId).Delete()


```