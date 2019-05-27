---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7002995c98e7b918f04422a82703906c85958c74
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476016"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  accountEnabled: true,
  addIns: [
    {
      id: "id-value",
      type: "type-value",
      properties: [
        {
          key: "key-value",
          value: "value-value"
        }
      ]
    }
  ],
  appDisplayName: "appDisplayName-value",
  appId: "appId-value",
  appOwnerOrganizationId: "appOwnerOrganizationId-value",
  appRoleAssignmentRequired: true
};

let res = await client.api('/servicePrincipals/{id}')
    .version('beta')
    .update({servicePrincipal : servicePrincipal});

```