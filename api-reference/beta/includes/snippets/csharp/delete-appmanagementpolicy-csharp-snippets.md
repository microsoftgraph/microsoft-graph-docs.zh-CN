---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ae5b4ea6dc133533bdc6dbbe2997d8efee8d88e
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.AppManagementPolicies["{appManagementPolicy-id}"]
    .Request()
    .DeleteAsync();

```