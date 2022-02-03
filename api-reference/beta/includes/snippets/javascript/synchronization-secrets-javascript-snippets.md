---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b4f1f7ed8b14af063434fefa3bb614e0a07f8d2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348764"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const secrets = {
    value: [
        {
            key: 'BaseAddress',
            value: 'user@domain.com'
        },
        {
            key: 'SecretToken',
            value: 'password-value'
        },
        {
            key: 'SyncNotificationSettings',
            value: '{\"Enabled\':false,\'DeleteThresholdEnabled\':false}"
        },
        {
            key: 'SyncAll',
            value: 'false'
        }
    ]
};

await client.api('/servicePrincipals/{id}/synchronization/secrets')
    .version('beta')
    .put(secrets);

```