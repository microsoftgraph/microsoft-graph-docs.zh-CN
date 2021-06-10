---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad4228aa422e7e6d0cfb26f287f05b73e51bde20
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentMultiple = {
    '@odata.type': '#microsoft.graph.unifiedRoleAssignmentMultiple',
    displayName: 'My test role assignment 1',
    description: 'My role assignment description',
    roleDefinitionId: 'b5c08161-a7af-481c-ace2-a20a69a48fb1',
    principalIds: ['f8ca5a85-489a-49a0-b555-0a6d81e56f0d', 'c1518aa9-4da5-4c84-a902-a31404023890']
};

await client.api('/roleManagement/cloudPC/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignmentMultiple);

```