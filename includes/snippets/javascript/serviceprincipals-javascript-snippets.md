---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ce3446a6ab4fb659945a49a10f693d3a3d39525
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = Content-type: appRoleAssignments/json

{
  principalId: "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  principalType: "User",
  appRoleId:"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  resourceId:"b00c693f-9658-4c06-bd1b-c402c4653dea"
};

let res = await client.api('/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments')
    .version('beta')
    .post(appRoleAssignment);

```