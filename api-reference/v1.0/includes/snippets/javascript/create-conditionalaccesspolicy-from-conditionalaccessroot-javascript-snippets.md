---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34888372115b01516f19200dd83bb9da57efb225
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565937"
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
            includeGroups: ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"],
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