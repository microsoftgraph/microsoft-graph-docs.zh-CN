---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d84b0843ddd3949a8b127468329b85b045ca8512
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2xIdentityUserFlow = {
    id: 'Partner',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 1,
    identityProviders: [
        {
            id: 'Facebook-OAuth',
            type: 'Facebook',
            name: 'Facebook'
        }
    ]
};

await client.api('/identity/b2xUserFlows')
    .version('beta')
    .post(b2xIdentityUserFlow);

```