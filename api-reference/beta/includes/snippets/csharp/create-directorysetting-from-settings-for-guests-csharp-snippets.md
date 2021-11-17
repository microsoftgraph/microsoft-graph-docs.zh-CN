---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5009d9ea58fb2667fe94f25c20ceb52a4ae728da
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = new GroupSetting
{
    DisplayName = "Group.Unified.Guest",
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