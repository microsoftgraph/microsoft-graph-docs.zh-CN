---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de038e38b5bf33195eaedb5e256a8fac1cbb1fa9be21295a2ece5f031029d587
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902782"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentResourceRoles = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentResourceRoles
    .Request()
    .GetAsync();

```