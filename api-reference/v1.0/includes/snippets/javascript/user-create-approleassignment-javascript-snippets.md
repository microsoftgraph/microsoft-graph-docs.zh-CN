---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e343cb61a12cf6d89e3f28592e9d831293db2fd2
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333384"
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

let res = await client.api('/users/{id}/appRoleAssignments')
    .post(appRoleAssignment);

```