---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57e5bfc1fdd8d2b5ff90d23570110bce4ca6b93f
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514619"
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
            Value = "true"
        }
    }
};

await graphClient.Groups["{group-id}"].Settings["{groupSetting-id}"]
    .Request()
    .UpdateAsync(groupSetting);

```