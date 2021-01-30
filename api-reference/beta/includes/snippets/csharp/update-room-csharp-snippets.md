---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 340900ce0e32b4600e7f22d8fd1ca0ea1cfa685f
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059703"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = new Room
{
    Nickname = "Conf Room",
    Building = "1",
    Label = "100",
    Capacity = 50,
    IsWheelChairAccessible = false
};

await graphClient.Places["cf100@contoso.com"]
    .Request()
    .UpdateAsync(place);

```