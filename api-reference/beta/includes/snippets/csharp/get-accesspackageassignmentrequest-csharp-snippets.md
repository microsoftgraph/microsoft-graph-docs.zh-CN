---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c1a99ef6eb420b74ce1eb9d4a89af4f235db46e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810125"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests["{accessPackageAssignmentRequest-id}"]
    .Request()
    .GetAsync();

```