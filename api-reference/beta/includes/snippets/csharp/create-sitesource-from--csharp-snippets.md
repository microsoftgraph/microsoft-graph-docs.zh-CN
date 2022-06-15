---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50379f0e9698860946da4f308886131da975f8c1
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092455"
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

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"].SiteSources
    .Request()
    .AddAsync(siteSource);

```