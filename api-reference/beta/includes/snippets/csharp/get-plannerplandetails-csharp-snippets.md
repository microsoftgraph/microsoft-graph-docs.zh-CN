---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f52164487a1e88a858c0c326edfbde1b5acc25b4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616929"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlanDetails = await graphClient.Planner.Plans["xqQg5FS2LkCp935s-FIFm2QAFkHM"].Details
    .Request()
    .GetAsync();

```