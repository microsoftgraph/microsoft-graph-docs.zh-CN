---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e399176f8c3363cfa83b1ac979f0bd0a3e2c89a09de7aa4a0518bfa121b45d62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161433"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cIdentityUserFlow = {
    id: 'UserFlowWithAPIConnector',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 1,
    apiConnectorConfiguration: {
        postFederationSignup: {
            '@odata.id': '{apiConnectorId}'
        },
        postAttributeCollection: {
            '@odata.id': '{apiConnectorId}'
        }
    }
};

await client.api('/identity/b2cUserFlows')
    .version('beta')
    .post(b2cIdentityUserFlow);

```