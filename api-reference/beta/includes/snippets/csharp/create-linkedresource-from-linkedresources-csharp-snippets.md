---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61b65aac689dcaa32ab722bd07d65889e581f72a
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48375710"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var linkedResource = new LinkedResource
{
    WebUrl = "https://microsoft.com",
    ApplicationName = "Microsoft",
    DisplayName = "Microsoft",
    ExternalId = "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
};

await graphClient.Me.Todo.Lists["dfsdc-f9dfdfs-dcsda9"].Tasks["e2dc-f9cce2-dce29"].LinkedResources
    .Request()
    .AddAsync(linkedResource);

```