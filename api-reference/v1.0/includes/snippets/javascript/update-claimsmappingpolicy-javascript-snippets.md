---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e44c5d99430f8a500fbc2f487e5b6d6a1a6fa00bdf5733189d7f646cce7a696b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
  definition: [
    'definition-value'
  ],
  displayName: 'displayName-value',
  isOrganizationDefault: true
};

await client.api('/policies/claimsMappingPolicies/{id}')
    .update(claimsMappingPolicy);

```