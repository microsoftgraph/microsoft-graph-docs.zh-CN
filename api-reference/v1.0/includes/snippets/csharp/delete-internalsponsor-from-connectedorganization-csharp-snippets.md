---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b56d91b1040577357bb73e06cf04cd361b6f8c4c
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61544915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"].ExternalSponsors["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```