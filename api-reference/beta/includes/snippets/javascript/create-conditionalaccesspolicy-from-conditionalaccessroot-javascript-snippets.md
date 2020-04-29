---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1f4f7150395a123dbda449f3a2174b13936ec0a
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43935070"
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
            includeGroups: ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"],
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