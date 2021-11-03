---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c2d1a5f669c3ad9f48a5126513201eb7cbd9072
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2021
ms.locfileid: "60676802"
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
                restrictForAppsCreatedAfterDateTime: '2021-04-01T10:37:00Z'
            },
            {
                restrictionType: 'passwordLifetime',
                maxLifetime: 'P4DT12H30M5S',
                restrictForAppsCreatedAfterDateTime: '2019-01-01T10:37:00Z'
            },
            {
                restrictionType: 'symmetricKeyAddition',
                maxLifetime: null,
                restrictForAppsCreatedAfterDateTime: '2021-04-01T10:37:00Z'
            },
            {
                restrictionType: 'symmetricKeyLifetime',
                maxLifetime: 'P40D',
                restrictForAppsCreatedAfterDateTime: '2015-04-01T10:37:00Z'
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