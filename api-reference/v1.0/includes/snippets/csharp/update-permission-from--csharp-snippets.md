---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f352a26d3a19a6b66b5bcd98d18b899b4318e1bf
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = new Permission
{
    Roles = new List<String>()
    {
        "read"
    }
};

await graphClient.Sites["{sitesId}"].Permissions["{permissionId}"]
    .Request()
    .UpdateAsync(permission);

```