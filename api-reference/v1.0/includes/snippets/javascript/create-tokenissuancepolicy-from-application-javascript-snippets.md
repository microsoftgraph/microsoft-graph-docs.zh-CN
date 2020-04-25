---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41c2772cf866870a6bf91278437460c8ae005319
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  @odata.id:"https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
};

let res = await client.api('/applications/{id}/tokenIssuancePolicies/$ref')
    .post(tokenIssuancePolicy);

```