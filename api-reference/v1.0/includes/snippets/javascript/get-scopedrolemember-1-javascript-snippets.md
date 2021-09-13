---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83f6ac04401a3ced22c340b9481e6650e35c752a1e4ac775cfafa00aacb5169d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMembership = await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .get();

```