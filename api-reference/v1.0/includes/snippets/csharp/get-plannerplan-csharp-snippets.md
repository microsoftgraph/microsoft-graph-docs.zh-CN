---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 591968b1c0ebf0331209497025a4787646b5e5a80d1cb4447e80ad8771d0b34e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104304"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlan = await graphClient.Planner.Plans["{plannerPlan-id}"]
    .Request()
    .GetAsync();

```