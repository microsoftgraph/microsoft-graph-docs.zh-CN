---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a316279059cd431e2e7fa3e8f97a4ce2f4aa5c5f
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceEnvironments = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceEnvironments
    .Request()
    .Filter("originSystem eq 'SharePointOnline'")
    .GetAsync();

```