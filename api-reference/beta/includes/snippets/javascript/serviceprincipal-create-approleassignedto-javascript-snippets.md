---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bdd1640d0a7fa58c1ff7de44d1c2c5cb5fe5df6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = {
  principalId: "principalId-value",
  resourceId: "resourceId-value",
  appRoleId: "appRoleId-value"
};

let res = await client.api('/servicePrincipals/{id}/appRoleAssignedTo')
    .version('beta')
    .post(appRoleAssignment);

```