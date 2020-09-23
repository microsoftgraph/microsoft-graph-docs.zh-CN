---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f0ac3e7838e8d4c56819c4800db5731e1434ef2
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroup = new ExternalGroup
{
    Id = "31bea3d537902000",
    DisplayName = "Contoso Marketing",
    Description = "The product marketing team"
};

await graphClient.External.Connections["contosohr"].Groups
    .Request()
    .AddAsync(externalGroup);

```