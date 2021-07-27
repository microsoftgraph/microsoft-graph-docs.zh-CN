---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27bfc4207e1c703040cb86468f89c1ed634b7339
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580111"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = new Microsoft.Graph.ExternalConnectors.ExternalConnection
{
    Id = "contosohr",
    Name = "Contoso HR",
    Description = "Connection to index Contoso HR system"
};

await graphClient.External.Connections
    .Request()
    .AddAsync(externalConnection);

```