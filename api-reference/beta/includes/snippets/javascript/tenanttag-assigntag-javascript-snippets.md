---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f489f612ebe488dd66967d833d271abbfc01b6266c3c8772683022e68ddf7d9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161553"
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