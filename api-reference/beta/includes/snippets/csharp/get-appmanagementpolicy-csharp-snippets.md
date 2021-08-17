---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dc7907e52b9c03231db5a71869d672b7d9a3ce0
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appManagementPolicy = await graphClient.Policies.AppManagementPolicies["{appManagementPolicy-id}"]
    .Request()
    .GetAsync();

```