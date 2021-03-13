---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79a395ea5e4fb9b9877fe9ad1e02cd3005f87c20
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recipients = new List<DriveRecipient>()
{
    new DriveRecipient
    {
        Email = "john@contoso.com"
    },
    new DriveRecipient
    {
        Email = "ryan@external.com"
    }
};

var roles = new List<String>()
{
    "read"
};

await graphClient.Shares["{sharedDriveItem-id}"].Permission
    .Grant(roles,recipients)
    .Request()
    .PostAsync();

```