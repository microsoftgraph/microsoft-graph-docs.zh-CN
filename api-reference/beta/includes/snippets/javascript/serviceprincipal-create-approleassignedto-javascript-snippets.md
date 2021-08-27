---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 772539f003dbc9b884a87cef8176f2d65c71361a81248da79d25640a48440bea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = {
  principalId: '33ad69f9-da99-4bed-acd0-3f24235cb296',
  resourceId: '9028d19c-26a9-4809-8e3f-20ff73e2d75e',
  appRoleId: 'ef7437e6-4f94-4a0a-a110-a439eb2aa8f7'
};

await client.api('/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignedTo')
    .version('beta')
    .post(appRoleAssignment);

```