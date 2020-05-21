---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d85222308cb7f02abd57a2c2c4adea25e89379a6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334031"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/appRoleAssignedTo/{id}')
    .version('beta')
    .delete();

```