---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 785c7f50c44bfbbbfeee2539a37cf04cdd1a2255
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719454"
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
  isOrganizationDefault: true,
  type: "type-value"
};

let res = await client.api('/policies/tokenIssuancePolicies/{id}')
    .update(tokenIssuancePolicy);

```