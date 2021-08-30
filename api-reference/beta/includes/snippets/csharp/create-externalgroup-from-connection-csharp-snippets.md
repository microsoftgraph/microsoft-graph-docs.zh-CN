---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 798f2227f9624f25a78cad2cbba5e925a6199283565ccd37c1d3d5d4e5c8a701
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220809"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroup = new Microsoft.Graph.ExternalConnectors.ExternalGroup
{
    Id = "31bea3d537902000",
    DisplayName = "Contoso Marketing",
    Description = "The product marketing team"
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups
    .Request()
    .AddAsync(externalGroup);

```