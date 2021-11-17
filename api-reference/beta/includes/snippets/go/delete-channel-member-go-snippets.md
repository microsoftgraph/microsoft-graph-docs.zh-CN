---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9e42d78c1dc3e03eda42330538437af22e25e95
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975900"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
channelId := "channel-id"
conversationMemberId := "conversationMember-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).MembersById(&conversationMemberId).Delete(options)


```