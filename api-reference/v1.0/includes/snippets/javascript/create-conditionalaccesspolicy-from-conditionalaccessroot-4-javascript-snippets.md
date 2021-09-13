---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67893435fe8e5d19de7b083f95777f97a63b861bb4da9b406aef17e3a209a0a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    displayName: 'Require MFA to EXO from non-compliant devices.',
    state: 'enabled',
    conditions: {
        applications: {
            includeApplications: [
                '00000002-0000-0ff1-ce00-000000000000'
            ]
        },
        users: {
            includeGroups: ['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba']
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
    .post(conditionalAccessPolicy);

```