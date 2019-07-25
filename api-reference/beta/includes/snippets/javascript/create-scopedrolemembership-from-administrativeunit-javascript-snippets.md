---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b2b6a3f9b4b0240d1d6bd7f4210c7282c7040a0a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710623"
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