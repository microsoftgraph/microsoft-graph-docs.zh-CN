---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6083a6b2a844c18be6c9f26b599873fb59699631
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59110504"
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
    isEnabled: true
};

await client.api('/roleManagement/directory/roleDefinitions')
    .post(unifiedRoleDefinition);

```