---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20649078c41dd2201ec5fb1003ef3492d6aea433
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60927060"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var noncustodialDataSource = new Microsoft.Graph.Ediscovery.NoncustodialDataSource
{
    ApplyHoldToSource = true,
    DataSource = new UserSource
    {
        Email = "adelev@contoso.com"
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].NoncustodialDataSources
    .Request()
    .AddAsync(noncustodialDataSource);

```