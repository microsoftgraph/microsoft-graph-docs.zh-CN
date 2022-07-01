---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79b2f39594927421af77b90a2bf048ca8007bad4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66604499"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var crossTenantAccessPolicy = new CrossTenantAccessPolicy
{
    AllowedCloudEndpoints = new List<String>()
    {
        "microsoftonline.us",
        "partner.microsoftonline.cn"
    }
};

await graphClient.Policies.CrossTenantAccessPolicy
    .Request()
    .UpdateAsync(crossTenantAccessPolicy);

```