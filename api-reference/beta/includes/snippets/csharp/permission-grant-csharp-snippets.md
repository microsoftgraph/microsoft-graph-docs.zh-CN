---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd42f5258a31a8cd4fc921d86a46e4807a4344a9eefd050ca7e24e6c14df4064
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215805"
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