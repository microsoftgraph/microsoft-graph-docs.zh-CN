---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 998e2c651551bc858058575cccabbe8ddddf4f7a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442762"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantTag = {
  tenantIds: [
    'String'
  ]
};

await client.api('/tenantRelationships/managedTenants/tenantTags/{tenantTagId}/unassignTag')
    .version('beta')
    .post(tenantTag);

```