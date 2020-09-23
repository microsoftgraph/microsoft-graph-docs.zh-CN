---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18e48b88f2372973f08212012ac013a985e9b2c6
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230743"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    displayName: "Require MFA to EXO from non-complaint devices.",
    state: "enabled",
    conditions: {
        applications: {
            includeApplications: [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        users: {
            includeGroups: ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        },
        devices: {
            includeDeviceStates: [
                "All"
            ],
            excludeDeviceStates: [
                "Compliant"
            ]
        }
    },
    grantControls: {
        operator: "OR",
        builtInControls: [
            "mfa"
        ]
    }
};

let res = await client.api('/identity/conditionalAccess/policies')
    .version('beta')
    .post(conditionalAccessPolicy);

```