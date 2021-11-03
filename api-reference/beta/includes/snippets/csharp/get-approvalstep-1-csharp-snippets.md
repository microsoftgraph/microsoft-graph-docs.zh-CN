---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f086ae31c868c6058fede9086ec7d04e52bf66c8766fd0fa1a8a17f523ca188
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var steps = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals["{approval-id}"].Steps
    .Request()
    .GetAsync();

```