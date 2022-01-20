---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d37c7a300624baa1a6aac379a2e293f65d8422c4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089921"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var linkedResource_v2 = new LinkedResource_v2
{
    WebUrl = "https://microsoft.com",
    ApplicationName = "Microsoft",
    DisplayName = "Microsoft Web page",
    ExternalId = "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
};

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].LinkedResources["{linkedResource_v2-id}"]
    .Request()
    .UpdateAsync(linkedResource_v2);

```