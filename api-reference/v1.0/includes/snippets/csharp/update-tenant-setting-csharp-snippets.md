---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98f36abb3d088cd04bb5925b89231c325003760b
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514643"
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