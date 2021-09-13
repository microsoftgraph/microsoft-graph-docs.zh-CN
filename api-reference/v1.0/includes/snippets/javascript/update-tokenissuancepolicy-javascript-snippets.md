---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f434910292d2adda52638b88563dfa9c7b61cb2a82f640c24e47a0f17b8ab59c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  definition: [
    'definition-value'
  ],
  displayName: 'displayName-value',
  isOrganizationDefault: true
};

await client.api('/policies/tokenIssuancePolicies/{id}')
    .update(tokenIssuancePolicy);

```