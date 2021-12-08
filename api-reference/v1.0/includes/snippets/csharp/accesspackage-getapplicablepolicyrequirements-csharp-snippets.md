---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5a2f8acbb06fed7f7b6040fd2ed164706dda54e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334909"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"]
    .GetApplicablePolicyRequirements()
    .Request()
    .PostAsync();

```