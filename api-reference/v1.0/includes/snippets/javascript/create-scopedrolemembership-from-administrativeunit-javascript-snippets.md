---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26a2039660cfcf978bf8b955e3fb91f48afdecbe
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223430"
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

let res = await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers')
    .post(scopedRoleMembership);

```