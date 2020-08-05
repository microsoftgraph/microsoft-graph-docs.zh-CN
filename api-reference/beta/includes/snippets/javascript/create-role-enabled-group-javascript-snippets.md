---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d47af37d4e0dd2d37ca6a4b5d7c28c32f9ac90d3
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "Group assignable to a role",
  displayName: "Role assignable group",
  groupTypes: [
    "Unified"
  ],
  isAssignableToRole: true,
  mailEnabled: true,
  securityEnabled: true,
  mailNickname: "contosohelpdeskadministrators",
  "visibility" : "Private"
};

let res = await client.api('/groups')
    .version('beta')
    .post(group);

```