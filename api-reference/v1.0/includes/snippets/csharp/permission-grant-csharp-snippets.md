---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29efcb266954cb7d3326fc679fb2d6cb9b479173
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124887"
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

await graphClient.Shares["{encoded-sharing-url}"].Permission
    .Grant(roles,recipients)
    .Request()
    .PostAsync();

```