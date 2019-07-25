---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 248228537a7aa1946e553fc0a641d8a5b8057364
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appRoleAssignments/{id}')
    .version('beta')
    .get();

```