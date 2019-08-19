---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a6ad8dde1e5abf3225d7b3755309dbb1a475b181
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignment = {
    principalId:"a98eb769-7bd4-4489-86f6-ad96e1d58b62",
    roleDefinitionId:"b0f54661-2d74-4c50-afa3-1ec803f12efe",
    resourceScope:"/"
};

let res = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .post({unifiedRoleAssignment : unifiedRoleAssignment});

```