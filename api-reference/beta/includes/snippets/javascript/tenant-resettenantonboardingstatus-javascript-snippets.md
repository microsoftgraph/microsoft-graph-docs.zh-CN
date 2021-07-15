---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a10a52eb8c2972d672a4b9ab1c806f56401b63f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440426"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/tenantRelationships/managedTenants/tenants/{tenantId}/resetTenantOnboardingStatus')
    .version('beta')
    .post();

```