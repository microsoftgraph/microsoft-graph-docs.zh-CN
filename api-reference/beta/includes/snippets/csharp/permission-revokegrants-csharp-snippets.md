---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2db98c03d2317a21c82673c3a41107866e34f44e9eda51ae8a2f667b6246da04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220267"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var grantees = new List<DriveRecipient>()
{
    new DriveRecipient
    {
        Email = "ryan@contoso.com"
    }
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Permissions["{permission-id}"]
    .RevokeGrants(grantees)
    .Request()
    .PostAsync();

```