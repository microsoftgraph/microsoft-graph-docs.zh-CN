---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2a7aba5146a729ef989fb779e813bd1ec2ef84a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784309"
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
            id: 'Facebook-OAuth',
            type: 'Facebook',
            Name: 'Facebook'
        }
    ]
};

await client.api('/identity/b2cUserFlows')
    .version('beta')
    .post(b2cIdentityUserFlow);

```