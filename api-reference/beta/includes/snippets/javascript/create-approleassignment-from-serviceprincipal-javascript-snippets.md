---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3e88431ec71fdd5ae78e14117747b3655967e4c1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725287"
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

let res = await client.api('/servicePrincipals/{id}/appRoleAssignments')
    .version('beta')
    .post({appRoleAssignment : appRoleAssignment});

```