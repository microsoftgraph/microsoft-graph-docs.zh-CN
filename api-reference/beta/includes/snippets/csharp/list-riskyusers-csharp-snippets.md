---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f2bcd041605a03129da2c1dd23f7c33069dac493
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521163"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUsers = await graphClient.RiskyUsers
    .Request()
    .GetAsync();

```