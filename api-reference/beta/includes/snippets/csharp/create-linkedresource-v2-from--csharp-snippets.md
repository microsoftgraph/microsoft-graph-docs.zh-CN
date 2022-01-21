---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1a2e9017faba94c3d1e09dbb807303925066d11
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124149"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var linkedResource_v2 = new LinkedResource_v2
{
    WebUrl = "https://microsoft.com",
    ApplicationName = "Microsoft",
    DisplayName = "Microsoft",
    ExternalId = "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
};

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].LinkedResources
    .Request()
    .AddAsync(linkedResource_v2);

```