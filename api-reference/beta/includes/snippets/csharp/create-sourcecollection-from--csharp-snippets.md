---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f52f2b08bcfca083bc04f00b5b69a7ab5f80a1057af22e2dd7bde3879d2471a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333035"
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