---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2099fff6c344d73c9ef3577963f245c77f3ed0a9fc0b3d7a119cb910165217a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328714"
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

var expirationDateTime = "2018-07-15T14:00:00Z";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Invite(recipients,requireSignIn,roles,sendInvitation,message,expirationDateTime,password)
    .Request()
    .PostAsync();

```