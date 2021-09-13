---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c92aca7077027d6c58bde8ef0411a99a804f73a82a0e1ba156b00328598c5c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904137"
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

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Invite(recipients,requireSignIn,roles,sendInvitation,message,expirationDateTime,password)
    .Request()
    .PostAsync();

```