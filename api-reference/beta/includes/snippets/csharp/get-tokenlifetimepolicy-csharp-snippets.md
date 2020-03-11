---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 904d8605493f40fd05b35210d31d983d2a69e072
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicy = await graphClient.Policies.TokenLifetimePolicies["{id}"]
    .Request()
    .GetAsync();

```