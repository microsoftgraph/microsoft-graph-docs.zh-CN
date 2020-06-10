---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2562155ed2ab1316e90940d0c9c117d289774757
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681822"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySetting = new DirectorySetting
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"directorySetting", "{\"displayName\":\"displayName-value\",\"templateId\":\"templateId-value\",\"values\":[{\"name\":\"name-value\",\"value\":\"value-value\"}]}"}
    }
};

await graphClient.Groups["{id}"].Settings
    .Request()
    .AddAsync(directorySetting);

```