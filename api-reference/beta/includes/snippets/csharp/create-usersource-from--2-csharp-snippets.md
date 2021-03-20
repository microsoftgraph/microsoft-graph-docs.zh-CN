---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bac599b74143c4faf31c5c96f017e72a77743d0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSource = new Microsoft.Graph.Ediscovery.UserSource
{
    Email = "adelev@contoso.com",
    IncludedSources = Microsoft.Graph.Ediscovery.SourceType.Mailbox
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds["{ediscovery.legalHold-id}"].UserSources
    .Request()
    .AddAsync(userSource);

```