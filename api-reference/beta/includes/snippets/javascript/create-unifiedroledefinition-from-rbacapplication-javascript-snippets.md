---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 706fd4491b0584d728da49499bc796abcd4ad383
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798456"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleDefinition = {
  description: 'Update basic properties of application registrations',
  displayName: 'Application Registration Support Administrator',
  rolePermissions: 
    [
        {
            allowedResourceActions: 
            [
                'microsoft.directory/applications/basic/read'
            ]
        }
    ],
    isEnabled: 'true'
};

await client.api('/roleManagement/directory/roleDefinitions')
    .version('beta')
    .post(unifiedRoleDefinition);

```