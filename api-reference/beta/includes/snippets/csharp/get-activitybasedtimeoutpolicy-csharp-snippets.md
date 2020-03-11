---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a53f5f075076adf797370dc0a4ba6b268b717b8
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityBasedTimeoutPolicy = await graphClient.Policies.ActivityBasedTimeoutPolicies["{id}"]
    .Request()
    .GetAsync();

```