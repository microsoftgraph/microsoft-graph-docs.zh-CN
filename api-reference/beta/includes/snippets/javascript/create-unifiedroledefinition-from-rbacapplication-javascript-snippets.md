---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 338f16b625d17cea2aad3bae6538dabdd759fdb9
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleDefinition = {
  description: "Update basic properties of application registrations",
  displayName: "Application Registration Support Administrator",
  rolePermissions:
    [
        {
            allowedResourceActions: 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ],
    "isEnabled" : "true"
};

let res = await client.api('/roleManagement/directory/roleDefinitions')
    .version('beta')
    .post({unifiedRoleDefinition : unifiedRoleDefinition});

```