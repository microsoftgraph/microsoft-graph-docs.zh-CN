---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 260f8720459a270073ecdbcd41c4b7d8aa71eebb516774da4ef828b9c3f881c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103769"
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