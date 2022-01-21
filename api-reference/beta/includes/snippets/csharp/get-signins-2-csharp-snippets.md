---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9e43128b6fc95a16cc5f7751ab6c2aab39d3d21
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095914"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("top", "10")
};

var signIns = await graphClient.AuditLogs.SignIns
    .Request( queryOptions )
    .Filter("startsWith(appDisplayName,'Azure')")
    .GetAsync();

```