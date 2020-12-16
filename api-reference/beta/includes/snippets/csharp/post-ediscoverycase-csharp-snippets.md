---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80517145b3dd337873a51530c4be00ca1733af87
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692770"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @case = new Case
{
    DisplayName = "My Case 1"
};

await graphClient.Compliance.Ediscovery.Cases
    .Request()
    .AddAsync(@case);

```