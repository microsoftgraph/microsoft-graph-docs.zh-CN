---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a73d0b3dffe52bfd4d814d623457b6aa92e0d92accf94b7b28d32a49fe56e1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220196"
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