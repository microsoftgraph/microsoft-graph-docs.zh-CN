---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6c8d30ed440794485675cb5b82e813531baea985725230e52e8d3c020a18883
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333691"
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