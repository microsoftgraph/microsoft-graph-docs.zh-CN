---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc931e7c6606ecaf249d71abe5035cc9bc289574a6db21d5a22d7a8a79d43a4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378547"
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