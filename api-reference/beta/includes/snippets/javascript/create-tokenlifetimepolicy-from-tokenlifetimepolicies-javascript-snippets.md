---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: accbc3972213f90827f38df7bba1c3b175460393f7d111a7da91a8625ac90bb6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903281"
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

await client.api('/policies/tokenLifetimePolicies')
    .version('beta')
    .post(tokenLifetimePolicy);

```