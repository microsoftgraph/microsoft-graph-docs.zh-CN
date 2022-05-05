---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61586dc828cf8e8e039aee3a04c7db174e7abe6f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const delegatedAdminAccessAssignment = {
  accessDetails: {
    unifiedRoles: [
      {
        roleDefinitionId: '88d8e3e3-8f55-4a1e-953a-9b9898b8876b'
      },
      {
        roleDefinitionId: '44367163-eba1-44c3-98af-f5787879f96a'
      },
      {
        roleDefinitionId: '729827e3-9c14-49f7-bb1b-9608f156bbb8'
      }
    ]
  }
};

await client.api('/tenantRelationships/delegatedAdminRelationships/5e5594d3-6f82-458b-b567-77db4811f0cd-00000000-0000-0000-0000-000000001234/accessAssignments/da9d6cf90-083a-47dc-ace2-1da98be3f344')
    .version('beta')
    .update(delegatedAdminAccessAssignment);

```