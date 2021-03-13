---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7966a1465964d9e1b9df04c46762b2a446c74320
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
  '@odata.type':'#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration',
  state: 'enabled',
  defaultLifetimeInMinutes: 60,
  defaultLength: 8,
  minimumLifetimeInMinutes: 60,
  maximumLifetimeInMinutes: 1440,"
  isUsableOnce":false,
  includeTargets: [
        {
            targetType: 'group',
            id: 'all_users',
            isRegistrationRequired: false,
            useForSignIn: true
        }
    ]
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass')
    .version('beta')
    .update(authenticationMethodConfiguration);

```