---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8192da4f3666398a270a23f521fc2b384c6ad90
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodsPolicy = {
    '@odata.context': 'https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy',
    authenticationMethodConfigurations: [
        {
            '@odata.type': '#microsoft.graph.fido2AuthenticationMethodConfiguration',
            id: 'Fido2',
            state: 'disabled',
            isSelfServiceRegistrationAllowed: false,
            isAttestationEnforced: false,
            keyRestrictions: {
                isEnforced: false,
                enforcementType: 'block',
                aaGuids: []
            }
        }
    ]
};

await client.api('/policies/authenticationMethodsPolicy')
    .update(authenticationMethodsPolicy);

```