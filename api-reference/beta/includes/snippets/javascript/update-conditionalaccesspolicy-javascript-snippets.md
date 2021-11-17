---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08232273bdbddec082775a8aa34b2f703e09e1550dbd0b39e78a7edc800e6e1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105235"
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
    .version('beta')
    .update(conditionalAccessPolicy);

```