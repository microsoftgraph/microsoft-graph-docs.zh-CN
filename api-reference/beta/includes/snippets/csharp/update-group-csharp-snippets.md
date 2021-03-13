---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72e3e725faee0c5c290934643010ce9b57d28c73
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785576"
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