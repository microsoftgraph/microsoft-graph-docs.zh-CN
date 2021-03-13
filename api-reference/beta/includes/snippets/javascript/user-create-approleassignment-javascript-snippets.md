---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23e13c874edd6f6e587d322173cc07474faae676
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780398"
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
    .version('beta')
    .post(appRoleAssignment);

```