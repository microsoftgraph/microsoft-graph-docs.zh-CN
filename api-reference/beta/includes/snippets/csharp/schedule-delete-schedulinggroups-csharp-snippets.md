---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8131581e2842444032347cc99e150c15422f9112
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35725623"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamId}"].Schedule.SchedulingGroups["{schedulingGroupId}"]
    .Request()
    .DeleteAsync();

```