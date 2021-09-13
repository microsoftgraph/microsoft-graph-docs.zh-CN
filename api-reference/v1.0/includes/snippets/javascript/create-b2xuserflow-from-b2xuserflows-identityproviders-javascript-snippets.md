---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bbab7e46045574f53adc725be90ff348ed2f60047229ade6f845f8c7b3be1bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332431"
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
    .post(b2xIdentityUserFlow);

```