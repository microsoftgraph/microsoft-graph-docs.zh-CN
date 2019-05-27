---
description: 自动生成的文件。 不修改
ms.openlocfilehash: baf088394085c2b2186025c3c82ef007a515946b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441470"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityDetail = await graphClient.Reports.GetOffice365GroupsActivityDetail('D7')
    .Request()
    .GetAsync();

```