---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84b7045bc52969960e0b511beedc6a150b4737c18d78b6bd9224b8fa5bca4bd8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var invitation = new Invitation
{
    InvitedUserEmailAddress = "yyy@test.com",
    InviteRedirectUrl = "https://myapp.contoso.com"
};

await graphClient.Invitations
    .Request()
    .AddAsync(invitation);

```