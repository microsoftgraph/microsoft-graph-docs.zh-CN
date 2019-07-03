---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ab63d70b639c3a4b5ff83bf207f9a41f6d0c7e05
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466762"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTaskDetails = await graphClient.Planner.Tasks["{task-id}"].Details
    .Request()
    .GetAsync();

```