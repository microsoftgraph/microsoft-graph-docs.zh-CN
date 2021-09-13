---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f142ed2c597acf570a99a2fa5d1d9f527d96863
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignment = {
    '@odata.type': '#microsoft.graph.unifiedRoleAssignment',
    principalId: '6b937a9d-c731-465b-a844-2d5b5368c161',
    roleDefinitionId: '9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3',
    directoryScopeId: '/661e1310-bd76-4795-89a7-8f3c8f855bfc'
};

await client.api('/roleManagement/directory/roleAssignments')
    .post(unifiedRoleAssignment);

```