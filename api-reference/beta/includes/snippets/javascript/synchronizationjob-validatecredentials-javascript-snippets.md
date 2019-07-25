---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9bd2d6024438dffb75c384642dd83c8ae9844fce
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateCredentials = {
    credentials: [ 
        { key: "UserName", value: "user@domain.com" },
        { key: "Password", value: "password-value" }
    ]
};

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials')
    .version('beta')
    .post(validateCredentials);

```