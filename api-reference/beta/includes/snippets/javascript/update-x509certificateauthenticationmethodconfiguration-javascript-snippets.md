---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a2e190ccc5bbfce4bcfa42c1d4df81f6b33160b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
    '@odata.type': '#microsoft.graph.x509CertificateAuthenticationMethodConfiguration',
    id: 'X509Certificate',
    state: 'enabled',
    certificateUserBindings: [
        {
            x509CertificateField: 'PrincipalName',
            userProperty: 'onPremisesUserPrincipalName',
            priority: 1
        }
    ],
    authenticationModeConfiguration: {
        x509CertificateAuthenticationDefaultMode: 'x509CertificateMultiFactor',
        rules: [
            {
                x509CertificateRuleType: 'issuerSubject',
                identifier: 'CN=ContosoCA,DC=Contoso,DC=org ',
                x509CertificateAuthenticationMode: 'x509CertificateMultiFactor'
            },
            {
                x509CertificateRuleType: 'policyOID',
                identifier: '1.2.3.4',
                x509CertificateAuthenticationMode: 'x509CertificateMultiFactor'
            }
        ]
    },
    includeTargets: [
        {
            targetType: 'group',
            id: 'all_users',
            isRegistrationRequired: false
        }
    ]
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate')
    .version('beta')
    .update(authenticationMethodConfiguration);

```