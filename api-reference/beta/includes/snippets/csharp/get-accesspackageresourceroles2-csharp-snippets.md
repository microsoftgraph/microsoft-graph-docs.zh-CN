---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5f0bbac9a88c8cec02e8ef1ee1e066b779a8fba
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439247"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRoles = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalog-id}"].AccessPackageResourceRoles
    .Request()
    .Filter("(originSystem eq 'SharePointOnline' and accessPackageResource/id eq '53c71803-a0a8-4777-aecc-075de8ee3991')")
    .Select("displayName,originId")
    .GetAsync();

```