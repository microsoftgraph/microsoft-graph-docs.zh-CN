---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8d674fad5d2e6fd6d33efb94349299b45792094
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994725"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = new ExternalConnection
{
    Id = "contosohr",
    Name = "Contoso HR",
    Description = "Connection to index Contoso HR system"
};

await graphClient.External.Connections
    .Request()
    .AddAsync(externalConnection);

```