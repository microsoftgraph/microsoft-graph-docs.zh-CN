---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d771befe45948074f75ea8e439662c5014c630e5
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461601"
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
    ]
};

let res = await client.api('/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a')
    .version('beta')
    .update({unifiedRoleDefinition : unifiedRoleDefinition});

```