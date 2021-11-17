---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46c64e89496477a6c4fa41ac01b3137c137d907b2952989c80a262c04e5fcdaa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902791"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequests = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .Request()
    .Filter("(requestState eq 'PendingApproval')")
    .Expand("requestor($expand=connectedOrganization)")
    .GetAsync();

```