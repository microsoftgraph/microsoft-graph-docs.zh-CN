---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ccfc9c42ec07f91fdf185781742cbacbe2c1437
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53578865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var verifiedPublisherId = "1234567";

await graphClient.Applications["{application-id}"]
    .SetVerifiedPublisher(verifiedPublisherId)
    .Request()
    .PostAsync();

```