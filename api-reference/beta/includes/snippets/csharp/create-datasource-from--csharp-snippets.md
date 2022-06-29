---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd86551a0949cee4d0e861057db64956c2e12f60
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440211"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataSource = new SiteSource
{
    Site = new Site
    {
        WebUrl = "https://contoso.sharepoint.com/sites/SecretSite"
    }
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"].AdditionalSources
    .Request()
    .AddAsync(dataSource);

```