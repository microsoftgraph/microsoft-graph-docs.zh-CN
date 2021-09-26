---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2eb993162dea58e2739c45e10f0b6d65b4d14e51165bbee5c9e0f01689408562
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277441"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    AssignedLabels = new List<AssignedLabel>()
    {
        new AssignedLabel
        {
            LabelId = "45cd0c48-c540-4358-ad79-a3658cdc5b88"
        }
    }
};

await graphClient.Groups["{group-id}"]
    .Request()
    .UpdateAsync(group);

```