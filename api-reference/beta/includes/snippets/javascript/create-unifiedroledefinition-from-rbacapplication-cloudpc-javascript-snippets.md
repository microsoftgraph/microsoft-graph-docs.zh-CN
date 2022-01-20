---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5202d6659946f8464326feb4dbd2cfe011bb59d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleDefinition = {
  description: 'An example custom role',
  displayName: 'ExampleCustomRole',
  rolePermissions: 
    [
        {
            allowedResourceActions: 
            [
                'Microsoft.CloudPC/CloudPCs/Read'
            ]
        }
    ],
    condition: 'null'
};

await client.api('/roleManagement/cloudPc/roleDefinitions')
    .version('beta')
    .post(unifiedRoleDefinition);

```