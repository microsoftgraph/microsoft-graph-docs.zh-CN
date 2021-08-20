---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c22c3802fc2e31bd1f8ef58cd926d68d55347f0
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.MobileAppManagementPolicies["{mobilityManagementPolicy-id}"]
    .Request()
    .DeleteAsync();

```