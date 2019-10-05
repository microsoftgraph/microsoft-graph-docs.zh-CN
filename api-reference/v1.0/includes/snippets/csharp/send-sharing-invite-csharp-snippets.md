---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5aa8014d84af658b73974de3f2e2ca8f640b4ce4
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402802"
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
    .Invite(recipients,requireSignIn,roles,sendInvitation,message)
    .Request()
    .PostAsync();

```