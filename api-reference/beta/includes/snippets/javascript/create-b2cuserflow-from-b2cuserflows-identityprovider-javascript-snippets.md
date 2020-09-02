---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15ac9e727d44ca84020b8ba5dbb4d383a7428efe
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cIdentityUserFlow = {
    id: "Customer",
    userFlowType: "signUpOrSignIn",
    userFlowTypeVersion: 3,
    identityProviders: [
        {
            id: "Facebook-OAuth",
            type: "Facebook",
            Name: "Facebook"
        }
    ]
};

let res = await client.api('/identity/b2cUserFlows')
    .version('beta')
    .post(b2cIdentityUserFlow);

```