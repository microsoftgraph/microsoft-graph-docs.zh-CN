---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff15be6032da790565eeb96e8fd0961169c94d13
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442713"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantTag = {
  displayName: 'Onboarding',
  description: 'Tenants that we are currently onboarding'
};

await client.api('/tenantRelationships/managedTenants/tenantTags/{tenantTagId}')
    .version('beta')
    .update(tenantTag);

```