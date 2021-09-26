---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2957415700bc22873d4f13e365099d6ab3661b9
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cIdentityUserFlow = {
    id: 'Customer',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 3,
    identityProviders: [
        {
            id: 'Facebook-OAuth'
        }
    ]
};

await client.api('/identity/b2cUserFlows')
    .version('beta')
    .post(b2cIdentityUserFlow);

```