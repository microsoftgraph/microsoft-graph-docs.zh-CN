---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bbc84604b82087b9c5ced72264994c142f4b8c54
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636586"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = {
  creationTimestamp: "2016-10-19T10:37:00Z",
  principalDisplayName: "principalDisplayName-value",
  principalId: "principalId-value",
  principalType: "principalType-value",
  resourceDisplayName: "resourceDisplayName-value"
};

let res = await client.api('/appRoleAssignments/{id}')
    .version('beta')
    .update(appRoleAssignment);

```