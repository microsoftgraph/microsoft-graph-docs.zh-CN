---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92e45a2697a9c28d870cfc5c3b6c8cd9cc0b745a9eb187a8eee56c882cb49376
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279355"
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

await graphClient.Connections["{externalConnectors.externalConnection-id}"].Items["{externalConnectors.externalItem-id}"]
    .Request()
    .UpdateAsync(externalItem);

```