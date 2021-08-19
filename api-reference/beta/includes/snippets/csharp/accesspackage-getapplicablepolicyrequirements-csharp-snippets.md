---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5a2f8acbb06fed7f7b6040fd2ed164706dda54e
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384108"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"]
    .GetApplicablePolicyRequirements()
    .Request()
    .PostAsync();

```