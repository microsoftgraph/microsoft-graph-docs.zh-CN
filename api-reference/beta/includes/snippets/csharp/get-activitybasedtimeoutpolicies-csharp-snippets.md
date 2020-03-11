---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65ca6e12909343d42e8deda0e3bef083cfb31d71
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityBasedTimeoutPolicies = await graphClient.Policies.ActivityBasedTimeoutPolicies
    .Request()
    .GetAsync();

```