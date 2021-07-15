---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0714cbe0750d0f3a0ce8edd86332c81ef91de12
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442074"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantTag = {
  displayName: 'Support',
  description: 'Tenants that have purchased extended support'
};

await client.api('/tenantRelationships/managedTenants/tenantTags')
    .version('beta')
    .post(tenantTag);

```