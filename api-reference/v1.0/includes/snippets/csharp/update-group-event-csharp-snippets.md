---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fdf7267983b422bb3000cc29628f4116a603d6dc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509588"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    Location = new Location
    {
        DisplayName = "Conf Room 2"
    }
};

await graphClient.Groups["01d4ee64-15ce-491e-bad1-b91aa3223df4"].Calendar.Events["AAMkADZlAAAAABERAAA="]
    .Request()
    .UpdateAsync(@event);

```