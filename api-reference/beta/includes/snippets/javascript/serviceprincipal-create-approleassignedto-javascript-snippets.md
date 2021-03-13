---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01f636536bbbe52faad0a47b72d4ea3ad770c4ac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798021"
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