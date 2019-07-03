---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 388e743d70a81b77cc29d1a92d5727e535e9ad3f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users.Delta()
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.JobTitle,
             e.MobilePhone 
             })
    .GetAsync();

```