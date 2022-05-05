---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bdd0cd8a1759461487e862a84cca42a557d060c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205431"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const delegatedAdminRelationship = {
  displayName: 'Contoso admin relationship',
  duration: 'P730D',
  customer: {
    tenantId: '4b827261-d21f-4aa9-b7db-7fa1f56fb163',
    displayName: 'Contoso subsidiary Inc'
  },
  accessDetails: {
    unifiedRoles: [
      {
        roleDefinitionId: '29232cdf-9323-42fd-ade2-1d097af3e4de'
      },
      {
        roleDefinitionId: '3a2c62db-5318-420d-8d74-23affee5d9d5'
      }
    ]
  }
};

await client.api('/tenantRelationships/delegatedAdminRelationships')
    .version('beta')
    .post(delegatedAdminRelationship);

```