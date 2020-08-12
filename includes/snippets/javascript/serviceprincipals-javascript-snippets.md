---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a7969abf092212c6ae3d36657520415e903ef92
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = Content-type: appRoleAssignments/json

{
  principalId: "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
  principalType: "User",
  appRoleId:"454dc4c2-8176-498e-99df-8c4efcde41ef",
  resourceId:"f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
};

let res = await client.api('/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/appRoleAssignments')
    .post(appRoleAssignment);

```