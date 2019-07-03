---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b2b6a3f9b4b0240d1d6bd7f4210c7282c7040a0a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const scopedRoleMembership = {
  roleId: "roleId-value",
  roleMemberInfo: {
    id: "id-value"
  }
};

let res = await client.api('/administrativeUnits/{id}/scopedRoleMembers')
    .version('beta')
    .post({scopedRoleMembership : scopedRoleMembership});

```