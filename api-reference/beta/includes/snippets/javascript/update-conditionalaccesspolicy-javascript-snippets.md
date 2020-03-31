---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dffcc38748cab00ac0fb9c5d8c08cb01a9fcf40a
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    conditions: {
        signInRiskLevels: [
            "high",
            "medium",
            "low",
        ]
    }
};

let res = await client.api('/identity/conditionalAccess/policies/{id}')
    .version('beta')
    .update(conditionalAccessPolicy);

```