---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f18e445a1a2f3efdd754aa2680cca599702df92f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481048"
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