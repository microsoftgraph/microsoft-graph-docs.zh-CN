---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4c4c548228bb8130e5e60e5c00aa268f10b43f4a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var program = new Program
{
    DisplayName = "testprogram3",
    Description = "test description"
};

await graphClient.Programs
    .Request()
    .AddAsync(program);

```