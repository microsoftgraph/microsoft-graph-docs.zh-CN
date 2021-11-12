---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2faa175fbe921266add8a63a3e2cc32c1a9c50ea9fdcd6f941fff02cd66a13c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279502"
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