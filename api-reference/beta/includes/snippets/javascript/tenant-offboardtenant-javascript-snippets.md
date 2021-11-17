---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6712ef428b38c0fa50460db7ebc947d0a97074d272252a9a87156e079246e015
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274363"
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