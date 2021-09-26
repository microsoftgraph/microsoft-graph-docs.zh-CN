---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b9ec27046993c9368f18ab0c5791f05b7aa48d35d0022d73af3d528822d4e22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162048"
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

await graphClient.Groups["{group-id}"].Settings
    .Request()
    .AddAsync(directorySetting);

```