---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2db2f47789953c64aee85fcee50a3937a0942bd0cafdf3658c9e966847f4b6f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103973"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRoster = new PlannerRoster
{
};

await graphClient.Planner.Rosters
    .Request()
    .AddAsync(plannerRoster);

```