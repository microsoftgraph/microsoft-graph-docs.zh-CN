---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0e26dc343cefdd7f9b4b0e7bf74fb5270e2e8b8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797919"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "Architecture Discussion",
    Description = "This channel is where we debate all future architecture plans",
    MembershipType = ChannelMembershipType.Standard,
    CreatedDateTime = DateTimeOffset.Parse("2020-03-14T11:22:17.067Z"),
    AdditionalData = new Dictionary<string, object>()
    {
        {"@microsoft.graph.channelCreationMode", "migration"}
    }
};

await graphClient.Teams["{team-id}"].Channels
    .Request()
    .AddAsync(channel);

```