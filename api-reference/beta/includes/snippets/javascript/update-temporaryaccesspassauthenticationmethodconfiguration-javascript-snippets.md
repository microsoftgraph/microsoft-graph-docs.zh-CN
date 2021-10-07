---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3454773cf4c5e1ed0836f792e832bac576272fd20bad60f6f22214c2c5c03eec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103825"
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