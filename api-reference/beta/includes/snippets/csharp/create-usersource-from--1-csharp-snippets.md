---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27db73fd6d43e6a054778d23a834fe9d021561e90e08531c784191ded1706c61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161498"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSource = new Microsoft.Graph.Ediscovery.UserSource
{
    Email = "megan@contoso.com",
    IncludedSources = Microsoft.Graph.Ediscovery.SourceType.Mailbox | Microsoft.Graph.Ediscovery.SourceType.Site
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UserSources
    .Request()
    .AddAsync(userSource);

```