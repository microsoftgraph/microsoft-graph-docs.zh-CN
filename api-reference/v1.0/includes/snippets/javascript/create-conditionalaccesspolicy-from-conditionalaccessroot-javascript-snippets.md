---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3d3bcf98eab2b2cfbf89cf76e59a794d2319bb0
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    displayName: "Require MFA to EXO from non-compliant devices.",
    state: "enabled",
    conditions: {
        applications: {
            includeApplications: [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        users: {
            includeGroups: ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
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
    .post(conditionalAccessPolicy);

```