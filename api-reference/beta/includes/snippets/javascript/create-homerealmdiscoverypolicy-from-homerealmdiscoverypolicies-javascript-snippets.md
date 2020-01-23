---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5e28fd71dd20a699cbfb9d75d663b170dd6d064
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const policy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/homeRealmDiscoveryPolicies')
    .version('beta')
    .post(policy);

```