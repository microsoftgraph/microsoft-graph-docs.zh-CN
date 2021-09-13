---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97cb2d52be027db289dbe512f26950fc2864de91a7cebc42108966576b3fed85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332659"
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