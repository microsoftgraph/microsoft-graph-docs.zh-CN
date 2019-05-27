---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e75c28942a50ea791787e701ef38b819478dcc28
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recipients = new List<DriveRecipient>()
{
    new DriveRecipient
    {
        Email = "ryan@contoso.org"
    }
};

var message = "Here's the file that we're collaborating on.";

var requireSignIn = true;

var sendInvitation = true;

var roles = new List<String>()
{
    "write"
};

var password = "password123";

var expirationDateTime = 7/15/2018 2:00:00 PM;

await graphClient.Me.Drive.Items["{item-id}"]
    .Invite(requireSignIn,roles,sendInvitation,message,recipients,expirationDateTime,password)
    .Request()
    .PostAsync();

```