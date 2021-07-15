---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56000a0184b5aa838c208cca2fa845713b009675
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441964"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementActionTenantDeploymentStatuses = await graphClient.TenantRelationships.ManagedTenants.ManagementActionTenantDeploymentStatuses
    .Request()
    .GetAsync();

```