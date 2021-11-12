---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9dfe29aa36d38429cb08a121978e1cd32c608d5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60934641"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSource = new Microsoft.Graph.Ediscovery.SiteSource
{
    Site = new Site
    {
        WebUrl = "https://contoso.sharepoint.com/sites/HumanResources"
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].SiteSources
    .Request()
    .AddAsync(siteSource);

```