---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ef3e1787513204757af2ddf5013ebe164472cfb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802089"
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

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"].LinkedResources
    .Request()
    .AddAsync(linkedResource);

```