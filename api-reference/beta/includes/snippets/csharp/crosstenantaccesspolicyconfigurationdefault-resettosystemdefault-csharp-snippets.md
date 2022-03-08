---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 721c4bc8cb90430542154e52058132cfbc4bf387
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336422"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.CrossTenantAccessPolicy.Default
    .ResetToSystemDefault()
    .Request()
    .PostAsync();

```