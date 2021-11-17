---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f36707871ec6f3993cf8f0c5e164964d7eb1d297a7ad89e8feb19e6bf15bb55b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105501"
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
    ]
};

await client.api('/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a')
    .version('beta')
    .update(unifiedRoleDefinition);

```