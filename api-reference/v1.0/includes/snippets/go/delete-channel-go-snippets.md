---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49638888893dce20e422e81311b2ec583138d7c1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085448"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
channelId := "channel-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).Delete(options)


```