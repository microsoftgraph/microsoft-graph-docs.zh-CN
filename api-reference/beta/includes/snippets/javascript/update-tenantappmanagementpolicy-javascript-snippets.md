---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d45ab60720a356a6aec44263c66d6e1109a5df77
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394689"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantAppManagementPolicy = {
    isEnabled: true,
    applicationRestrictions: {
        passwordCredentials: [
            {
                restrictionType: 'passwordAddition',
                maxLifetime: null,
                restrictForAppsCreatedAfterDateTime: '2021-01-01T10:37:00Z'
            },
            {
                restrictionType: 'passwordLifetime',
                maxLifetime: 'P4DT12H30M5S',
                restrictForAppsCreatedAfterDateTime: '2017-01-01T10:37:00Z'
            },
            {
                restrictionType: 'symmetricKeyAddition',
                maxLifetime: null,
                restrictForAppsCreatedAfterDateTime: '2021-01-01T10:37:00Z'
            },
            {
                restrictionType: 'customPasswordAddition',
                maxLifetime: null,
                restrictForAppsCreatedAfterDateTime: '2015-01-01T10:37:00Z'
            },
            {
                restrictionType: 'symmetricKeyLifetime',
                maxLifetime: 'P40D',
                restrictForAppsCreatedAfterDateTime: '2015-01-01T10:37:00Z'
            }
        ],
        keyCredentials: [
            {
                restrictionType: 'asymmetricKeyLifetime',
                maxLifetime: 'P30D',
                restrictForAppsCreatedAfterDateTime: '2015-01-01T10:37:00Z'
            },
        ]
    }
};

await client.api('/policies/defaultAppManagementPolicy')
    .version('beta')
    .update(tenantAppManagementPolicy);

```