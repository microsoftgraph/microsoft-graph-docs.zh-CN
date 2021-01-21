---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4a378069ec1886cecd7e51f57c5104db49db364
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/claimsMappingPolicies/{id}')
    .update(claimsMappingPolicy);

```