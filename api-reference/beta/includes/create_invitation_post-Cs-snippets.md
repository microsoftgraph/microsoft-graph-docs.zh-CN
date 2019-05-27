---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ff3ee57a389310bc8fa1d7bd384e961710c4a4db
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34483350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var invitation = new Invitation
{
    InvitedUserEmailAddress = "yyy@test.com",
    InviteRedirectUrl = "https://myapp.com"
};

await graphClient.Invitations
    .Request()
    .AddAsync(invitation);

```