---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8153a6bee36864807641981f789a276f56acf3302b1acef107cf1204577a49b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158523"
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