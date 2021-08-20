---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc1e7059bd32a39b41b4cb2b97fe3caeeb91b02d143d4927d84056204a63f596
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902960"
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

await graphClient.Groups["{group-id}"].Calendar.Events["{event-id}"]
    .Request()
    .UpdateAsync(@event);

```