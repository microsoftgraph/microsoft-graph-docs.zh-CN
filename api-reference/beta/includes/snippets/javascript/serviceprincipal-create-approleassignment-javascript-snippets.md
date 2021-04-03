---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28a16d0e11f6fd84b95d0fd9b0b3f99a176377e2
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508144"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = {
  principalId: '9028d19c-26a9-4809-8e3f-20ff73e2d75e',
  resourceId: '8fce32da-1246-437b-99cd-76d1d4677bd5',
  appRoleId: '498476ce-e0fe-48b0-b801-37ba7e2685c6'
};

await client.api('/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignments')
    .version('beta')
    .post(appRoleAssignment);

```