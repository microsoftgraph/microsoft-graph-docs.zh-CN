---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76b6d02e628e8faa9809d0615525d9aeffc14d0c
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var linkedResource = new LinkedResource
{
    WebUrl = "http:://microsoft.com",
    ApplicationName = "Microsoft",
    DisplayName = "Microsoft",
    ExternalId = "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
};

await graphClient.Me.Todo.Lists["dfsdc-f9dfdfs-dcsda9"].Tasks["e2dc-f9cce2-dce29"].LinkedResources
    .Request()
    .AddAsync(linkedResource);

```