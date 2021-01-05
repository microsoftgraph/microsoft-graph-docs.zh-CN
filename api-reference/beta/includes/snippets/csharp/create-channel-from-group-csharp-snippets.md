---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b77de86ec897d5a702382c42e590f76db3020996
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753790"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "Architecture Discussion",
    Description = "This channel is where we debate all future architecture plans",
    MembershipType = ChannelMembershipType.Standard
};

await graphClient.Teams["57fb72d0-d811-46f4-8947-305e6072eaa5"].Channels
    .Request()
    .AddAsync(channel);

```