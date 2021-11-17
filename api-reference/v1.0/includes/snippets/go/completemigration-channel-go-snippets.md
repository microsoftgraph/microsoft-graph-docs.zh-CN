---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 154c6b59b1f5282e7f8df759967db006bfa106da
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974410"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
channelId := "channel-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).CompleteMigration().Post(options)


```