---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d73d61aa6b6467b8ed14a55b41b1fa6d046e63ec
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySetting = new DirectorySetting
{
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "CustomBlockedWordsList",
            Value = "Contoso"
        }
    }
};

await graphClient.Settings["{directorySetting-id}"]
    .Request()
    .UpdateAsync(directorySetting);

```