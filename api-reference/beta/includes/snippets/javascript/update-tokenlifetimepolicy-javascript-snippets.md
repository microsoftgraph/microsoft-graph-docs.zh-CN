---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1931b195137ca9a27a9d4d1cc35436667bbb1eff
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/tokenLifetimePolicies/{id}')
    .version('beta')
    .update(tokenLifetimePolicy);

```