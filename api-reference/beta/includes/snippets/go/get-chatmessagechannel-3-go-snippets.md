---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f0dfecec9f370c59213771739c7b27d65736eb5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287910"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
channelId := "channel-id"
chatMessageId := "chatMessage-id"
chatMessageId1 := "chatMessage-id1"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).MessagesById(&chatMessageId).RepliesById(&chatMessageId1).Get(nil)


```