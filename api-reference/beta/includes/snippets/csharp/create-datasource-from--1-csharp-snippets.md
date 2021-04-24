---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6128e9dac63139d6b84029ab2adf57855a01fdc7
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51987547"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataSource = new Microsoft.Graph.Ediscovery.UserSource
{
    Email = "badguy@contoso.com"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].AdditionalSources
    .Request()
    .AddAsync(dataSource);

```