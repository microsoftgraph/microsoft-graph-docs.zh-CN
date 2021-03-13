---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e33325f88d0c5404a6caa5228dfc0c56cba33c32
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783677"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySetting = new DirectorySetting
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"directorySetting", "{\"displayName\":\"displayName-value\",\"templateId\":\"templateId-value\",\"values\":[{\"name\":\"name-value\",\"value\":\"value-value\"}]}"}
    }
};

await graphClient.Groups["{group-id}"].Settings
    .Request()
    .AddAsync(directorySetting);

```