---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b365d539188d30dd20815345c359372f0bef488
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566059"
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
    .update(conditionalAccessPolicy);

```