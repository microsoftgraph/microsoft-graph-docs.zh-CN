---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ff3ee57a389310bc8fa1d7bd384e961710c4a4db
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738737"
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