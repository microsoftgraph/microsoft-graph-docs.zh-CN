---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01566cae87400209a8038b40f2fcbc5616bf99d9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783642"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = {
  principalId: 'principalId-value',
  resourceId: 'resourceId-value',
  appRoleId: 'appRoleId-value'
};

await client.api('/users/{id}/appRoleAssignments')
    .post(appRoleAssignment);

```