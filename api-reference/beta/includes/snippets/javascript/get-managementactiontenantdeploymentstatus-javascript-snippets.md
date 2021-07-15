---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4865bcf23bead96c7a79ac61953c2d2669acb6e4
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442601"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementActionTenantDeploymentStatus = await client.api('/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}')
    .version('beta')
    .get();

```