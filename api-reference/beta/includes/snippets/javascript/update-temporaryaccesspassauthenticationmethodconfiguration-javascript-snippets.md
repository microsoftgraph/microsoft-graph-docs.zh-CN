---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03548cae2b84103d47c928723a24fd6f29b0a9e4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
  @odata.type:"#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  state:"enabled",
  defaultLifetimeInMinutes:60,
  defaultLength:8,
  minimumLifetimeInMinutes:60,
  maximumLifetimeInMinutes:1440,"
  isUsableOnce":false,
  includeTargets: [
        {
            targetType: "group",
            id: "all_users",
            isRegistrationRequired: false,
            useForSignIn: true
        }
    ]
};

let res = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass')
    .version('beta')
    .update(authenticationMethodConfiguration);

```