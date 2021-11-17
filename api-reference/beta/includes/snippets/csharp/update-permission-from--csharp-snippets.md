---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b203f87e7809b7570d4f4495c540bfacb3722ca376d697bb48fecb1d8b2c3552
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333084"
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

await graphClient.Sites["{site-id}"].Permissions["{permission-id}"]
    .Request()
    .UpdateAsync(permission);

```