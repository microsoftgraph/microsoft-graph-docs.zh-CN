---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 384d4455e964a48c29f21de72aacf5b3a22f8552
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442566"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementIntent = await client.api('/tenantRelationships/managedTenants/managementIntents/{managementIntentId}')
    .version('beta')
    .get();

```