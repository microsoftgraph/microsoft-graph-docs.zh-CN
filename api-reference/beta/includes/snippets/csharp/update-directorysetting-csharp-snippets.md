---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8f513a42eb7aaeb3bdc81fa0893019bd1872d7927570ccaa590bcbfe8951bd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106459"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySetting = new DirectorySetting
{
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "name-value",
            Value = "value-value"
        }
    }
};

await graphClient.Settings["{directorySetting-id}"]
    .Request()
    .UpdateAsync(directorySetting);

```