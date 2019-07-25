---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5657fc920e1c31d8015bd711e14502375ec778d4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720052"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var program = new Program
{
    DisplayName = "testprogram3 new name"
};

await graphClient.Programs["7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"]
    .Request()
    .UpdateAsync(program);

```