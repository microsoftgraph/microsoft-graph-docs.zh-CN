---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13b1c77bbb4b1074c402e67b7712f6bad5f588fd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780830"
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