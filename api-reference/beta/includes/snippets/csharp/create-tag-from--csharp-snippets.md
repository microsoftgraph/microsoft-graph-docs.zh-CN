---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d3761da305fef29412969cc729f993050f8ee380c834e8a70e56773c0efdcb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tag = new Microsoft.Graph.Ediscovery.Tag
{
    DisplayName = "Privileged",
    Description = "The document is privileged",
    AdditionalData = new Dictionary<string, object>()
    {
        {"parent@odata.bind", "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"}
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags
    .Request()
    .AddAsync(tag);

```