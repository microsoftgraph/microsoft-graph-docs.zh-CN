---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e859230c904955517b6381a9aa6cc309a19c00ba
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441859"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantGroup = {
  tenantId: 'String'
};

await client.api('/tenantRelationships/managedTenants/tenantGroups/tenantSearch')
    .version('beta')
    .post(tenantGroup);

```