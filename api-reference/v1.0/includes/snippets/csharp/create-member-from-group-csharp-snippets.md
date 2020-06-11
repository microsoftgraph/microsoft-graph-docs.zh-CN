---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e0eec332cec42474872b1e8809881a959defafa
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"members@odata.bind", "[\"https://graph.microsoft.com/v1.0/directoryObjects/{id}\",\"https://graph.microsoft.com/v1.0/directoryObjects/{id}\",\"https://graph.microsoft.com/v1.0/directoryObjects/{id}\"]"}
    }
};

await graphClient.Groups["{id}"]
    .Request()
    .UpdateAsync(group);

```