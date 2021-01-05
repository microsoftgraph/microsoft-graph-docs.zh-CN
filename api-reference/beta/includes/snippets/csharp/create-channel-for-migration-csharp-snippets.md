---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03d61e7902fda22667e2151c40ab00af89cf06a3
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753791"
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

await graphClient.Teams["57fb72d0-d811-46f4-8947-305e6072eaa5"].Channels
    .Request()
    .AddAsync(channel);

```