---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 593d7e4787d8c75e5e94a7e8946e9f346f293fed
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336364"
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