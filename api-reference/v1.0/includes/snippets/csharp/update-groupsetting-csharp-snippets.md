---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84226b8bdad311f91a6e84d5a2bc6e55c4c31237
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947067"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = new GroupSetting
{
    DisplayName = "GroupSettings",
    TemplateId = "08d542b9-071f-4e16-94b0-74abb372e3d9",
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "AllowToAddGuests",
            Value = false
        }
    }
};

await graphClient.Groups["{id}"].Settings["{id}"]
    .Request()
    .UpdateAsync(groupSetting);

```