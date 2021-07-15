---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 303d747637f6adba30e0cf4a2486f3187c5e0607
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant')
    .version('beta')
    .post();

```