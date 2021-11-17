---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd32bdf77fbc38fc8adcc9f32d3fe408ea65bdcba8b2273f381d2c2d1714267a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163209"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignment = {
    '@odata.type': '#microsoft.graph.unifiedRoleAssignment',
    roleDefinitionId: 'c2cf284d-6c41-4e6b-afac-4b80928c9034',
    principalId: 'f8ca5a85-489a-49a0-b555-0a6d81e56f0d',
    directoryScopeId: '/'
};

await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignment);

```