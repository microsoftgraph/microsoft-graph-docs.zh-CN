---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6697f222fa2ac1830b58622032701a0bcfbf87e6cecb1d300db7c7fdf164f6c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceEnvironments = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceEnvironments
    .Request()
    .Filter("originSystem eq 'SharePointOnline'")
    .GetAsync();

```