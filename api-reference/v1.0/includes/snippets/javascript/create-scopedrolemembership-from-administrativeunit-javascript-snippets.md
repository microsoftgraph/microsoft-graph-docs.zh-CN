---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f9156be85dee51b969af75572acc22f24d18e16de17862c700a4d38f042a198
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105435"
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