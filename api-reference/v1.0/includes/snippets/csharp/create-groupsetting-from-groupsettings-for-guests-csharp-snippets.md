---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ae5c77acb7f8476fb50488e92c1e22c680cf232
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412694"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = new GroupSetting
{
    TemplateId = "08d542b9-071f-4e16-94b0-74abb372e3d9",
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "AllowToAddGuests",
            Value = "false"
        }
    }
};

await graphClient.Groups["{group-id}"].Settings
    .Request()
    .AddAsync(groupSetting);

```