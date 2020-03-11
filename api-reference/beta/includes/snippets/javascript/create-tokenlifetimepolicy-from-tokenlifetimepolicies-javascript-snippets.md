---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d843ce7eafab4f8034acd0d6913d8230dd1f3ac
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589289"
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

let res = await client.api('/policies/tokenLifetimePolicies')
    .version('beta')
    .post(tokenLifetimePolicy);

```