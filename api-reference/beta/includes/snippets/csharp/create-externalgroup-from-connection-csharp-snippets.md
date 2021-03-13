---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d2de86b0f580ab14af1c02ac81e71dd50bce56d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808113"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroup = new ExternalGroup
{
    Id = "31bea3d537902000",
    DisplayName = "Contoso Marketing",
    Description = "The product marketing team"
};

await graphClient.External.Connections["{externalConnection-id}"].Groups
    .Request()
    .AddAsync(externalGroup);

```