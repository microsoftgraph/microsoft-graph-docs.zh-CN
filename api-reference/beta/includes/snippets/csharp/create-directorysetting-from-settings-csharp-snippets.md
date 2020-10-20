---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f18e445a1a2f3efdd754aa2680cca599702df92f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610514"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySetting = new DirectorySetting
{
    TemplateId = "templateId-value",
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "name-value",
            Value = "value-value"
        }
    }
};

await graphClient.Settings
    .Request()
    .AddAsync(directorySetting);

```