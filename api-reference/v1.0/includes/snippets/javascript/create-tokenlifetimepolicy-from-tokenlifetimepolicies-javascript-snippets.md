---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6cf5e91202323a1de6046c801e7caf62bb2ba42462de0b059c56f3b195b815c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278193"
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
    .post(tokenLifetimePolicy);

```