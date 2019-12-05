---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 593d7e4787d8c75e5e94a7e8946e9f346f293fed
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37997038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = new Room
{
    Nickname = "Conf Room",
    Building = "1",
    Label = "100",
    Capacity = "50",
    IsWheelchairAccessible = false
};

await graphClient.Places["cf100@contoso.com"]
    .Request()
    .UpdateAsync(place);

```