---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6ab2213c5ad08274849a3c978d3e4fa05ad65050
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636614"
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
    .update(unifiedRoleDefinition);

```