---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7543603a01c86f1e7136c1ff609a1af33c521095
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573114"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = {
  principalId: 'cde330e5-2150-4c11-9c5b-14bfdc948c79',
  resourceId: '8e881353-1735-45af-af21-ee1344582a4d',
  appRoleId: '00000000-0000-0000-0000-000000000000'
};

await client.api('/users/cde330e5-2150-4c11-9c5b-14bfdc948c79/appRoleAssignments')
    .post(appRoleAssignment);

```