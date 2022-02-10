---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fc19d11d03bf32b74360a5a101470775be0813f
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageCatalog = new AccessPackageCatalog
{
    DisplayName = "Catalog One"
};

await graphClient.IdentityGovernance.EntitlementManagement.Catalogs["{accessPackageCatalog-id}"]
    .Request()
    .UpdateAsync(accessPackageCatalog);

```