---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1473f72092700c8ea6b8445f1f7f2e8692bc9ee2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026853"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
channelId := "channel-id"
chatMessageId := "chatMessage-id"
chatMessageId1 := "chatMessage-id1"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).MessagesById(&chatMessageId).RepliesById(&chatMessageId1).Get(options)


```