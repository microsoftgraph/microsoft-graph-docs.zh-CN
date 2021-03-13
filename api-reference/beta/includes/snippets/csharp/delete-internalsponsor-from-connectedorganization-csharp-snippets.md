---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bb510f8b30dc961f1581a97af255586d4fc202f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809296"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"].InternalSponsors["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```