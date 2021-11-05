---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c53b5764fe3df067d56e3aec3f138b125987a9b18d33e783a85976c44f2ebab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests["{accessPackageAssignmentRequest-id}"]
    .Request()
    .GetAsync();

```