---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8d8b690b41d72f97593f2c8739c50a716c94e8f
ms.sourcegitcommit: df2c52f84aae5d4fed641d7411ba547371f0eaad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2020
ms.locfileid: "44055578"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recipients = new List<DriveRecipient>()
{
    new DriveRecipient
    {
        Email = "ryan@contoso.com"
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

var expirationDateTime = "2018-07-15T14:00:00Z";

await graphClient.Me.Drive.Items["{item-id}"]
    .Invite(recipients,requireSignIn,roles,sendInvitation,message,expirationDateTime,password)
    .Request()
    .PostAsync();

```