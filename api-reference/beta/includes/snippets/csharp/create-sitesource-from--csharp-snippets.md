---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25a02740efbbc32735a115c014fc0289db2e7a23
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446698"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSource = new Microsoft.Graph.Security.SiteSource
{
    Site = new Site
    {
        WebUrl = "https://m365x809305.sharepoint.com/sites/Retail"
    }
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].LegalHolds["{security.ediscoveryHoldPolicy-id}"].SiteSources
    .Request()
    .AddAsync(siteSource);

```