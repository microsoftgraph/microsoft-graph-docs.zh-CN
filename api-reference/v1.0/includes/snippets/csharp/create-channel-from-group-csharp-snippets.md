---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3808ed99b700e48bebc34fcdd72b9deab1acbd65fa8f8844024b128fe23f7266
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333833"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "Architecture Discussion",
    Description = "This channel is where we debate all future architecture plans",
    MembershipType = ChannelMembershipType.Standard
};

await graphClient.Teams["{team-id}"].Channels
    .Request()
    .AddAsync(channel);

```