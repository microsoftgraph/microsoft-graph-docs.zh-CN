---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e76f941ff861d85945838bc1d1e2e9e6fafa78f1
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryNoncustodialDataSource = new Microsoft.Graph.Security.EdiscoveryNoncustodialDataSource
{
    DataSource = new SiteSource
    {
        Site = new Site
        {
            WebUrl = "https://m365x809305.sharepoint.com/sites/Design-topsecret"
        }
    }
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].NoncustodialDataSources
    .Request()
    .AddAsync(ediscoveryNoncustodialDataSource);

```