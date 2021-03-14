---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8a37b6ebec8527b3f09a1ca01de1a1f54d15b7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    conditions: {
        signInRiskLevels: [
            'high',
            'medium',
            'low',
        ]
    }
};

await client.api('/identity/conditionalAccess/policies/{id}')
    .update(conditionalAccessPolicy);

```