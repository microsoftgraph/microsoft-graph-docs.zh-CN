---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d0b1b46bbd453653dc559cea1536e375b1b5abf
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094912"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoverySearch = new Microsoft.Graph.Security.EdiscoverySearch
{
    DisplayName = "My search 2",
    Description = "My first search",
    ContentQuery = "(Author=\"edison\")",
    AdditionalData = new Dictionary<string, object>()
    {
        {"custodianSources@odata.bind", "[\"https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/userSources/43434642-3137-3138-3432-374142313639\",\"https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/siteSources/169718e3-a8df-449d-bef4-ee09fe1ddc5d\",\"https://graph.microsoft.com/beta/security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources('32e14fa4-3106-4bd2-a245-34bf0c718a7e')\"]"},
        {"noncustodialSources@odata.bind", "[\"https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/35393639323133394345384344303043\"]"}
    }
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches
    .Request()
    .AddAsync(ediscoverySearch);

```