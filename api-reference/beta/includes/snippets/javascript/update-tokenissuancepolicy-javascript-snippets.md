---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb7480cc0f17e6abbd78b95491a8e82c428774bf
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/tokenIssuancePolicies/{id}')
    .version('beta')
    .update(tokenIssuancePolicy);

```