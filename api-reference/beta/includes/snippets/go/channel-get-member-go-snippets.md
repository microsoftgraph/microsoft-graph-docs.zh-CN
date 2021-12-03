---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31a4298c117c678aa80cc9d4ea229a5a641c239b
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287930"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
channelId := "channel-id"
conversationMemberId := "conversationMember-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).MembersById(&conversationMemberId).Get(nil)


```