---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f76a9c8ee7b6e34bf07e1ed4bebaad21979e1db3
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373448"
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