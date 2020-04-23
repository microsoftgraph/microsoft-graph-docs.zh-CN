---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6049103f6e8ef0658c0a557db636ef1c6315ec74
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43770941"
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

await graphClient.Me.Drive.Items["{item-id}"]
    .Invite(recipients,requireSignIn,roles,sendInvitation,message,null,null)
    .Request()
    .PostAsync();

```