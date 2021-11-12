---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 309acfb48091b064539d490398abf4c1cac3c6b524196f9b987c941fe53add04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274172"
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