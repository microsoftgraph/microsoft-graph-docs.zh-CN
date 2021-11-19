---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d88daa832cb43596f7e5f16ba178b55012f96375
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103529"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalItem = new Microsoft.Graph.ExternalConnectors.ExternalItem
{
    Acl = new List<Microsoft.Graph.ExternalConnectors.Acl>()
    {
        new Microsoft.Graph.ExternalConnectors.Acl
        {
            Type = Microsoft.Graph.ExternalConnectors.AclType.Everyone,
            Value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
            AccessType = Microsoft.Graph.ExternalConnectors.AccessType.Grant
        }
    }
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Items["{externalConnectors.externalItem-id}"]
    .Request()
    .UpdateAsync(externalItem);

```