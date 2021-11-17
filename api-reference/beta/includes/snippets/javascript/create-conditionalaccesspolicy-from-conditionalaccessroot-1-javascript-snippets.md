---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 483fb50f11bc7e99647f31a21609e4618f98c5519d24a5826238c9e953137e8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    displayName: 'Access to EXO requires MFA',
    state: 'enabled',
    conditions: {
        clientAppTypes: [
            'mobileAppsAndDesktopClients',
            'browser'
        ],
        applications: {
            includeApplications: [
                '00000002-0000-0ff1-ce00-000000000000'
            ]
        },
        users: {
            includeGroups: ['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba']
        },
        locations: {
            includeLocations: [
                'All'
            ],
            excludeLocations: [
                'AllTrusted'
            ]
        }
    },
    grantControls: {
        operator: 'OR',
        builtInControls: [
            'mfa'
        ]
    }
};

await client.api('/identity/conditionalAccess/policies')
    .version('beta')
    .post(conditionalAccessPolicy);

```