---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efdfa981ed39b28cd4d8be1306fdc0fa051f5292
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346615"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.IdentityGovernance.EntitlementManagement.Assignments
    .Request()
    .GetAsync();

```