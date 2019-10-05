---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f76a9c8ee7b6e34bf07e1ed4bebaad21979e1db3
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "Architecture Discussion",
    Description = "This channel is where we debate all future architecture plans",
    MembershipType = ChannelMembershipType.Standard
};

await graphClient.Teams["{id}"].Channels
    .Request()
    .AddAsync(channel);

```