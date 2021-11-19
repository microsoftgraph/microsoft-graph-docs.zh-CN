---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6b634ab103d789e7e95404e3ccbbdb46a42e93e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodsPolicy = {
    '@odata.context': 'https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy',
    registrationEnforcement: {
    authenticationMethodsRegistrationCampaign: {
        snoozeDurationInDays: 1,
        state: 'enabled',
        excludeTargets: [],
        includeTargets: [
            {
                id: '3ee3a9de-0a86-4e12-a287-9769accf1ba2',
                targetType: 'group',
                targetedAuthenticationMethod: 'microsoftAuthenticator'
            }
        ]
      }
    },
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