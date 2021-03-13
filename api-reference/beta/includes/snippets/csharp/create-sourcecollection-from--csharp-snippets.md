---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 890854c2a76cb1633f833484151378ec12653a3a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceCollection = new Microsoft.Graph.Ediscovery.SourceCollection
{
    DisplayName = "Quarterly Financials search",
    ContentQuery = "subject:'Quarterly Financials'",
    AdditionalData = new Dictionary<string, object>()
    {
        {"custodianSources@odata.bind", "[\"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735\"]"}
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections
    .Request()
    .AddAsync(sourceCollection);

```