---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 716acd58af4754cb4a4352dca24839bfaa0cac3a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773562"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateCredentials = {
    credentials: [ 
        { key: 'UserName', value: 'user@domain.com' },
        { key: 'Password', value: 'password-value' }
    ]
};

await client.api('/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials')
    .version('beta')
    .post(validateCredentials);

```