---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02e6753c44e63d1cec6325de555381f1710ff61a3fa0d1b1e5487228d714fd4d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104901"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    displayName: 'Require MFA to EXO from non-complaint devices.',
    state: 'enabled',
    conditions: {
        applications: {
            includeApplications: [
                '00000002-0000-0ff1-ce00-000000000000'
            ]
        },
        users: {
            includeGroups: ['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba']
        },
        devices: {
            includeDevices: [
                'All'
            ],
            excludeDevices: [
                'Compliant'
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