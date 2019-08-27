---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fd33c460fe9e1a794f0f59e02f8a3480606317c9
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636689"
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
    .post(unifiedRoleDefinition);

```