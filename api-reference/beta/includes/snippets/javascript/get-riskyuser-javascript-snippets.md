---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9e69d7c8b1b4e960e086491879c38d2262d619a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441404"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUser = await client.api('/tenantRelationships/managedTenants/riskyUsers/{riskyUserId}')
    .version('beta')
    .get();

```