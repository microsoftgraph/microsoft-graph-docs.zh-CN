---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d23bd9f4edf628646f5decca24fdc2921290ee7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953222"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rosterPlans = await graphClient.Users["{user-id}"].Planner.RosterPlans
    .Request()
    .GetAsync();

```