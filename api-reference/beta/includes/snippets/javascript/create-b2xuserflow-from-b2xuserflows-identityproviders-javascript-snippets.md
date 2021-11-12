---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 405a4b25461f1616e068ab8e892bec2c2976756eb0370967ed767df0b99b59ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221114"
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