---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9fd20a6c9857ce384d58870e8b5946dd988541d
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475519"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var {id} = await graphClient.Policies["activityBasedTimeoutPolicies"].{id}
    .Request()
    .GetAsync();

```