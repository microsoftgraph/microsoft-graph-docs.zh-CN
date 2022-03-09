---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98f36abb3d088cd04bb5925b89231c325003760b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = new GroupSetting
{
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "AllowToAddGuests",
            Value = "false"
        }
    }
};

await graphClient.GroupSettings["{groupSetting-id}"]
    .Request()
    .UpdateAsync(groupSetting);

```