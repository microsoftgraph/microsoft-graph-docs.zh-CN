---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fad4162fdfcde8ab98e2fda03c841a0f653728e7e0d559e17cf66a2eb0527f5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicy = {
  definition: [
    'definition-value'
  ],
  displayName: 'displayName-value',
  isOrganizationDefault: true
};

await client.api('/policies/tokenLifetimePolicies/{id}')
    .version('beta')
    .update(tokenLifetimePolicy);

```