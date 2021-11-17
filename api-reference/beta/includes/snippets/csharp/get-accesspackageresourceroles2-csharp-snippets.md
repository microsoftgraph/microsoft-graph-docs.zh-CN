---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcb10460b9bb0fbcc11d72742db2719f890bd96c2e52cb1aa64c2623cfdedd3f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104175"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRoles = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalog-id}"].AccessPackageResourceRoles
    .Request()
    .Filter("(originSystem eq 'SharePointOnline' and accessPackageResource/id eq '53c71803-a0a8-4777-aecc-075de8ee3991')")
    .Select("displayName,originId")
    .GetAsync();

```