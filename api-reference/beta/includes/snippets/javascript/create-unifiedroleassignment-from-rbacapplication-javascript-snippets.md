---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9b8f0aaf0cb6ee8c115d3ba725bd4eb3d3a71643
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636638"
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
    .post(unifiedRoleAssignment);

```