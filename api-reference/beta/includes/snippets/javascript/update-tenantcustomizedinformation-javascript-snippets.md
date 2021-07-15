---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 694d5a0afe8f9c8fa4baa03120fedb1b4deed51d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantCustomizedInformation = {
  '@odata.type': '#microsoft.graph.managedTenants.tenantCustomizedInformation',
  tenantId: 'String',
  contacts: [
    {
      '@odata.type': 'microsoft.graph.managedTenants.tenantContactInformation'
    }
  ],
  website: 'String'
};

await client.api('/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}')
    .version('beta')
    .update(tenantCustomizedInformation);

```