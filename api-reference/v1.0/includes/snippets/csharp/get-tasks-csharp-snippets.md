---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ec219b73741e988b9e0e42f4b90e911eeca6369a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Planner.Tasks
    .Request()
    .GetAsync();

```