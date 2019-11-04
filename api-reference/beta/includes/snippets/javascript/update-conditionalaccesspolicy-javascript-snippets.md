---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a4f179c61ab340d1b78067c674ce6b44479b6c0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936708"
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

let res = await client.api('/conditionalAccess/policies/{id}')
    .version('beta')
    .update(conditionalAccessPolicy);

```