---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5186150a068bc9bce1069bf445a8769a781a7683
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appManagementPolicy = {
    displayName: 'Credential management policy',
    description: 'Cred policy sample',
    isEnabled: true,
    restrictions: {
            passwordCredentials: [
               {
                  restrictionType: 'passwordAddition',
                  maxLifetime: null,
                  restrictForAppsCreatedAfterDateTime: '2019-10-19T10:37:00Z'
               },
               {
                  restrictionType: 'passwordLifetime',
                  maxLifetime: 'P4DT12H30M5S',
                  restrictForAppsCreatedAfterDateTime: '2014-10-19T10:37:00Z'
               },
               {
                  restrictionType: 'symmetricKeyAddition',
                  maxLifetime: null,
                  restrictForAppsCreatedAfterDateTime: '2019-10-19T10:37:00Z'
               },
               {
                  restrictionType: 'symmetricKeyLifetime',
                  maxLifetime: 'P4D',
                  restrictForAppsCreatedAfterDateTime: '2014-10-19T10:37:00Z'
               }
            ],
            keyCredentials: [
               {
                  restrictionType: 'asymmetricKeyLifetime',
                  maxLifetime: 'P90D',
                  restrictForAppsCreatedAfterDateTime: '2014-10-19T10:37:00Z'
               }
            ]
         }
};

await client.api('/policies/appManagementPolicies')
    .version('beta')
    .post(appManagementPolicy);

```