---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af9c37b4fcf1d1b65e3592730b4a2de7d3840321
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const scopedRoleMembership = {
  roleId: 'roleId-value',
  roleMemberInfo: {
    id: 'id-value'
  }
};

await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers')
    .post(scopedRoleMembership);

```