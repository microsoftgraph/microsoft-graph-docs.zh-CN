---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d19a6b66b3a5fd8a121f609b8640fd89cdb2a05c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441747"
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

await client.api('/tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag')
    .version('beta')
    .post(tenantTag);

```