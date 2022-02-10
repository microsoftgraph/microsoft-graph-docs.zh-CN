---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c36adab131c7bf5c8106408ff5230af823e6cc7
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
    '@odata.type': '#microsoft.graph.x509CertificateAuthenticationMethodConfiguration',
    id: 'X509Certificate',
    state: 'disabled',
    certificateUserBindings: [{
            x509CertificateField: 'PrincipalName',
            userProperty: 'onPremisesUserPrincipalName',
            priority: 1
        },
        {
            x509CertificateField: 'RFC822Name',
            userProperty: 'userPrincipalName',
            priority: 2
        }
    ],
    authenticationModeConfiguration: {
        x509CertificateAuthenticationDefaultMode: 'x509CertificateSingleFactor',
        rules: []
    },
    includeTargets: [{
        targetType: 'group',
        id: 'all_users',
        isRegistrationRequired: false
    }]
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate')
    .version('beta')
    .update(authenticationMethodConfiguration);

```